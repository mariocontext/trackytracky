
<template>
  <div class="nuxt-holding-element">
    <GeneralHeader contextTriggerIsActive>
    <span slot="header-title">History</span>
    </GeneralHeader>

  <main class="container mx-auto px-4 mx-4 flex flex-col">
    <!-- Local and Global History tabs -->
    <div class="tabs container fixed mb-4 border-b-2 bg-white w-full text-xl">
      <span class="your-box-transaction tab inline-block uppercase p-4 border-b-4 border-primary cursor-pointer">Your box</span>
      <span class="global-transaction-tab inline-block uppercase p-4 cursor-pointer">Global</span>
    </div>
    <section class="transaction-listing my-16">

        <TransactionItem 
        v-for="item in items"
        :key="item.id"
        :item="item"
        />

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

  let nextItemId = 1

  export default {
    components: {
      GeneralHeader,
      TransactionItem
    },
    data () {
    return {
      items: [
          {
            id: nextItemId++,
            title: 'Transaction 1'
          },
          {
            id: nextItemId++,
            title: 'Transaction 2'
          },
          {
            id: nextItemId++,
            title: 'Transaction 3'
          },
          {
            id: nextItemId++,
            title: 'Transaction 4'
          },
          {
            id: nextItemId++,
            title: 'Transaction 5'
          },
          {
            id: nextItemId++,
            title: 'Transaction 6'
          },
          {
            id: nextItemId++,
            title: 'Transaction 7'
          },
          {
            id: nextItemId++,
            title: 'Transaction 8'
          },
          {
            id: nextItemId++,
            title: 'Transaction 9'
          },
          {
            id: nextItemId++,
            title: 'Transaction 10'
          }
			  ]
      }
    }
  }
</script>


