
<template>
  <div class="nuxt-holding-element">

    <GeneralHeader>
    <span slot="header-title">Settings</span>
    </GeneralHeader>

    <main class="min-h-screen flex flex-col mt-12 items-center">

      <!-- node info section -->
      <section class="node-info-area">
        <div class="node-info">
          <h2 class="text-lg">iMyn node 63</h2>
          <input class="inline" type="checkbox" name="testnet" value="yes">Test net</input>
        </div>
        <div class="firmware">
          <p>Firmware version 0.6.5.2</p>
          <input class="inline" type="checkbox" name="auto-update" value="yes">auto update</input>
          <button class="node-update-action bg-none border-none disabled">Update</button>
        </div>
        
      </section>

      <!-- current time section -->
      <section class="current-time-area">
        <h3>Current time</h3>
        <p>14:32:19 UTC</p>
        <button class="bg-transparent border-none">Change</button>
      </section>

      <!-- satellites -->
      <section class="satellites-section">
          <h3 class="my-4 text-center font-normal">GPS Satellites</h3>
          <div class="flex justify-between">

            <SatelliteItem>
              <span slot="satellite-id">1A</span>
              <span slot="satellite-strength">80%</span>
            </SatelliteItem>

            <SatelliteItem>
              <span slot="satellite-id">2A</span>
              <span slot="satellite-strength">40%</span>
            </SatelliteItem>

            <SatelliteItem>
              <span slot="satellite-id">3A</span>
              <span slot="satellite-strength">60%</span>
            </SatelliteItem>

          </div>

          <div class="location-coords mt-8 text-lg text-center">
            36°05'44.7"N 115°10'33.8"W
          </div>

          <button class="mt-4 uppercase text-center">Retry</button>
        
      </section>

      <form action="#">
        <label for="wifi-network">Wifi network</label>
          <select name="wifi-network" id="wifi-network">
              <option value="john" selected="selected">Johns Network</option>
              <option value="saab">Saab</option>
              <option value="opel">Opel</option>
              <option value="audi">Audi</option>
          </select>
      </form>

      <nuxt-link to="/summary" class="btn btn-primary wizard-button">Next</nuxt-link>

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
  import SatelliteItem from '~/components/SatelliteItem.vue'
  import GeneralHeader from '~/components/global/GeneralHeader.vue'
  export default {
    components: {
      SatelliteItem,
      GeneralHeader
    }
  }
</script>


