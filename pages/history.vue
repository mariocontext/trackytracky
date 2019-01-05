
<template>
  <div class="nuxt-holding-element">
    <GeneralHeader>
    <span slot="header-title">History</span>
    </GeneralHeader>

  <main class="container mx-auto p-4 m-4 flex flex-col">
    <!-- Local and Global History tabs -->
    <div class="tabs mb-4 border-b-2 text-xl">
      <span class="your-box-transaction tab inline-block uppercase p-4 border-b-4 border-primary cursor-pointer">Your box</span>
      <span class="global-transaction-tab inline-block uppercase p-4 cursor-pointer">Global</span>
    </div>
    <section class="transaction-listing">
        <TransactionItem>
        </TransactionItem>
    </section>

    </main>
  
  </div>
</template>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

</style>

<script>
  import GeneralHeader from '~/components/global/GeneralHeader.vue'
  import TransactionItem from '~/components/TransactionItem.vue'
  export default {
    components: {
      GeneralHeader,
      TransactionItem
    }
  }
</script>


