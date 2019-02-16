<template>
  <div class="nuxt-holding-element">

    <main class="min-h-screen flex flex-col mt-12 items-center">

      <h1>Location Setup</h1>
        <div class="location_icon mb-4">
          <svg width="150" height="150" viewBox="0 0 150 150" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M74.6056 118.307L74.9977 118.811L75.3927 118.309C82.0277 109.891 89.8573 98.9301 96.0309 87.813C102.194 76.7153 106.75 65.3855 106.75 56.25C106.75 38.7239 92.5261 24.5 75 24.5C57.4739 24.5 43.25 38.7239 43.25 56.25C43.25 65.2932 47.8702 76.6553 54.063 87.7899C60.2674 98.9452 68.0964 109.952 74.6056 118.307ZM75 136.749C74.9637 136.708 74.9248 136.664 74.8834 136.617C74.5643 136.256 74.0956 135.721 73.4989 135.028C72.3054 133.643 70.5996 131.626 68.5523 129.104C64.4572 124.058 58.9978 116.99 53.5395 108.9C48.0802 100.809 42.628 91.7037 38.5422 82.5837C34.4535 73.457 31.75 64.352 31.75 56.25C31.75 32.3386 51.0886 13 75 13C98.9114 13 118.25 32.3386 118.25 56.25C118.25 64.352 115.546 73.457 111.458 82.5837C107.372 91.7037 101.92 100.809 96.4605 108.9C91.0022 116.99 85.5428 124.058 81.4477 129.104C79.4004 131.626 77.6946 133.643 76.5011 135.028C75.9044 135.721 75.4357 136.256 75.1166 136.617C75.0752 136.664 75.0363 136.708 75 136.749Z" stroke="#607D8B"/>
          <path d="M90.125 56.25C90.125 64.6033 83.3533 71.375 75 71.375C66.6467 71.375 59.875 64.6033 59.875 56.25C59.875 47.8967 66.6467 41.125 75 41.125C83.3533 41.125 90.125 47.8967 90.125 56.25Z" stroke="#607D8B"/>
          </svg>
        </div>

        <section class="satellites-section flex flex-col items-center">
          <h3 class="my-4 text-center">GPS Satellites</h3>
          <div class="flex justify-between">

            <BaseSatelliteItem>
              <span slot="satellite-id">1A</span>
              <span slot="satellite-strength">80%</span>
            </BaseSatelliteItem>

            <BaseSatelliteItem>
              <span slot="satellite-id">2A</span>
              <span slot="satellite-strength">40%</span>
            </BaseSatelliteItem>

            <BaseSatelliteItem>
              <span slot="satellite-id">3A</span>
              <span slot="satellite-strength">60%</span>
            </BaseSatelliteItem>

          </div>

          <div class="location-coords mt-8 text-lg text-center">
            36°05'44.7"N 115°10'33.8"W
          </div>

          <button class="btn-tertiary mt-4">Retry</button>
        
        </section>


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
</script>


