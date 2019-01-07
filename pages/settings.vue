
<template>
  <div class="nuxt-holding-element">

    <GeneralHeader>
    <span slot="header-title">Settings</span>
    </GeneralHeader>

    <main class="settings-area min-h-screen max-w-sm mx-auto">

      <!-- node info section -->
      <section class="node-info-area box">
        <div class="node-info flex justify-between">
          <h2>iMyn node 63</h2>
          <div>
            <input type="checkbox" name="toggle-test-net" value="yes">Test net</input>
          </div>
        </div>
        <div class="firmware flex justify-between">
          <div>
            <p>Firmware version 0.6.5.2</p>
            <input type="checkbox" name="auto-update" value="yes">auto update</input>
          </div>
          <button class="node-update-action bg-none border-none disabled">Update</button>
        </div>
        
      </section>

      <!-- current time section -->
      <section class="current-time-area flex justify-between box">
        <div>
          <h3 class="title">Current time</h3>
          <p class="time-utc">14:32:19 UTC</p>
        </div>
        <button class="change-btn bg-transparent border-none">Change</button>
      </section>

      <!-- satellites -->
      <section class="satellites-section box">

          <h3 class="sat-title font-normal text-center">GPS Satellites</h3>

          <div class="satellite-list flex justify-center">

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

          <div class="location-coords text-lg text-center">
            <p>36°05'44.7"N 115°10'33.8"W</p>
            <button class="mt-4 uppercase text-center">Retry</button>
          </div>

      </section>

      <form class="wifi-choice box" action="#">
        <label for="wifi-network">Wifi network</label>
          <select name="wifi-network" id="wifi-network">
              <option value="john" selected="selected">Johns Network</option>
              <option value="saab">Saab</option>
              <option value="opel">Opel</option>
              <option value="audi">Audi</option>
          </select>
      </form>

      <nuxt-link to="/summary" class="wizard-button bg-basic btn btn-primary box">Next</nuxt-link>

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


