
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
    <section class="listing">
      <ul class="list-reset">
        <li>
          <div class="transaction-item-area flex items-center justify-between p-4 border-b-2 ">
            <div class="transaction-item-info max-w-md">
              <h4 class="mb-2 font-normal">transaction item title</h4>
              <p class="text-xs">summary info goes here Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod ipsa iusto qui quos soluta neque voluptates, dolorum corrupti atque dolorem? Veritatis, praesentium fugit? Molestias, sint facere. Quos iusto voluptatibus eius.</p>
            </div>
            <div class="transaction-more-details">
              <button class="border-none bg-none">Details</button>
            </div>
          </div>
        </li>
      </ul>
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
  export default {
    components: {
      GeneralHeader
    }
  }
</script>


