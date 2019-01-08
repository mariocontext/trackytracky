
<template>
  <div class="nuxt-holding-element">

    <GeneralHeader>
    <span slot="header-title">Settings</span>
    </GeneralHeader>

    <main class="settings-area min-h-screen max-w-sm mx-auto p-4">

      <!-- node info section -->
      <section class="node-info-area my-4">
        <div class="node-info mb-4 flex justify-between">
          <h2>iMyn node 63</h2>
          <div class="flex justify-end items-center">
            <span class="font-regular pr-4">Test net</span>
            <span class="toggler">
              <span class="toggle-active">
                <span class="toggle-btn">
                </span>
              </span>
            </span>
          </div>
        </div>
        <div class="firmware mt-4 flex justify-between">
          <div>
            <p>Firmware version 0.6.5.2</p>
            <input class="mt-4" type="checkbox" name="auto-update" value="yes" checked> auto update</input>
          </div>
          <button class="node-update-action opacity-50 cursor-not-allowed">Update</button>
        </div>
        
      </section>

      <!-- current time section -->
      <section class="current-time-area flex justify-between my-8">
        <div>
          <h3 class="title">Current time</h3>
          <p class="time-utc mt-4">14:32:19 UTC</p>
        </div>
        <button class="btn-tertiary">Change</button>
      </section>

      <!-- satellites -->
      <section class="satellites-section">

          <h3 class="sat-title">GPS Satellites</h3>

          <div class="satellite-list mt-4 -ml-1 flex justify-start">

            <SatelliteItem class="mr-4">
              <span slot="satellite-id">1A</span>
              <span slot="satellite-strength">80%</span>
            </SatelliteItem>

            <SatelliteItem class="mr-4">
              <span slot="satellite-id">2A</span>
              <span slot="satellite-strength">40%</span>
            </SatelliteItem>

            <SatelliteItem class="mr-4">
              <span slot="satellite-id">3A</span>
              <span slot="satellite-strength">60%</span>
            </SatelliteItem>

          </div>

          <div class="location-coords flex justify-between items-center">
            <p class="text-lg">36°05'44.7"N 115°10'33.8"W</p>
            <button class="btn-tertiary">Retry</button>
          </div>

      </section>

      <form class="wifi-choice" action="#">
        <label for="wifi-network">Wifi network</label>
          <select name="wifi-network" id="wifi-network">
              <option value="john" selected="selected">Johns Network</option>
            <option value="sarah">Sarah Network</option>
            <option value="open">Open wifi</option>
            <option value="6HDD-router">6HDD-router</option>
          </select>
      </form>

      <nuxt-link to="/summary" class="block wizard-button btn btn-primary pin-b mt-8 w-32 mx-auto">Next</nuxt-link>

    </main>
  
  </div>
</template>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

.toggler .toggle-active {
  @apply border rounded-full border-grey flex items-center cursor-pointer w-12 bg-primary justify-end;
}

.toggler .toggle-inactive {
  @apply border rounded-full border-grey flex items-center cursor-pointer w-12 justify-start;
}

.toggler .toggle-btn {
 @apply rounded-full border w-6 h-6 border-grey shadow-inner bg-white shadow;
}

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


