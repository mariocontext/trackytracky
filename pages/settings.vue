
<template>
  <div class="nuxt-holding-element">

    <GeneralHeader>
    <span slot="header-title">Settings</span>
    </GeneralHeader>

    <main class="settings-area min-h-screen max-w-sm mx-auto p-4">

      <!-- node info section -->
      <section class="node-info-area my-4">
        <div class="node-info mb-4 flex justify-between">
          <h2 class="font-light">iMyn node 63</h2>
          <div>
            <input type="checkbox" name="toggle-test-net" value="yes" checked> Test net</input>
          </div>
        </div>
        <div class="firmware mt-4 flex justify-between">
          <div>
            <p>Firmware version 0.6.5.2</p>
            <input class="my-2" type="checkbox" name="auto-update" value="yes"> auto update</input>
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
        <button class="change-btn bg-transparent border-none">Change</button>
      </section>

      <!-- satellites -->
      <section class="satellites-section">

          <h3 class="sat-title font-normal text-xl">GPS Satellites</h3>

          <div class="satellite-list mt-4 flex justify-start">

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

          <div class="location-coords text-lg flex justify-between items-center">
            <div class="font-regular">36°05'44.7"N 115°10'33.8"W</div>
            <button class="block uppercase text-center border-none">Retry</button>
          </div>

      </section>

      <form class="wifi-choice" action="#">
        <label for="wifi-network">Wifi network</label>
          <select name="wifi-network" id="wifi-network">
              <option value="john" selected="selected">Johns Network</option>
              <option value="saab">Saab</option>
              <option value="opel">Opel</option>
              <option value="audi">Audi</option>
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

.box {
  border:1px solid grey;
  margin: 1rem;
}

.settings-area {

}

.node-info-area {

}

.node-info {

}

.firmware {

}

.title {

}

.time-utc {

}

.change-button {

}

.current-time-area {

}


.satellites-section {

}

.sat-title {

}

.satellite-list {

}

.location-coords {

}

.wifi-choice {

}

.wizard-button {

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


