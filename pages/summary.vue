<template>
 <div class="nuxt-holding-element">

  <GeneralHeader>
   <span slot="header-title">Summary</span>
  </GeneralHeader>

  <main class="container mx-auto p-4 m-4 flex flex-col items-center">
    <section class="max-w-sm text-center">
      <h1>iMyn Node 63</h1>
      <!-- upload download area -->
      <div class="upload-download-area flex justify-around">
        <div>
          <p class="mb-2">32 Mbps</p>
          <h5>Upload</h5>
        </div>
        <div>
          <p class="mb-2">65 Mbps</p>
          <h5>Download</h5>
        </div>
      </div>
      <!-- latency area -->
      <h2 class="font-light mt-8 mb-4">Latency</h2>
      <div class="latency-area">
        <div class="local-global-latency flex justify-around">
          <div>
            <p class="mb-2 text-3xl">170 ms</p>
            <h5>Your Latency</h5>
          </div>
          <div>
            <p class="mb-2 text-3xl">300 ms</p>
            <h5>Global Latency</h5>
          </div>
        </div>
        <div class="global-average">
          <h4 class="my-4">Global average</h4>
          <div class="latency-measure">
            <svg width="303" height="50" viewBox="0 0 303 50" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect y="12" width="303" height="26" fill="#C4C4C4"/>
              <rect y="12" width="253" height="26" fill="#FF5722"/>
              <rect x="154" width="2" height="50" fill="black"/>
            </svg>
          </div>
          <p class="font-semibold">+48%</p>
        </div>
      </div>
    </section>


      <nuxt-link to="/history" class="btn btn-primary wizard-button">View History</nuxt-link>
    
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
