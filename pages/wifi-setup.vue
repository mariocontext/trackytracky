<template>
  <div class="nuxt-holding-element">

    <main class="min-h-screen flex flex-col mt-12 items-center">

      <h1>Wifi Setup</h1>
        <div class="wifi_icon mb-4">
            <svg width="138" height="98" viewBox="0 0 138 98" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M124.999 40.2471C93.832 9.4593 43.668 9.4593 12.5011 40.2471L0.708293 28.4543C38.4221 -8.81826 99.1403 -8.81785 136.792 28.454L124.999 40.2471ZM86.7906 78.4554L68.75 96.496L50.7104 78.4564C60.796 68.7431 76.766 68.7446 86.7906 78.4554ZM99.9981 65.248C82.6447 48.2715 54.8553 48.2715 37.5019 65.248L25.709 53.455C49.6096 29.9939 87.9528 29.9946 111.791 53.4545L99.9981 65.248Z" stroke="#607D8B"/>
          </svg>

        </div>
        <form class="mt-4 w-64 max-w-md" action="#">
          <label for="wifi-network">Select a wifi network</label>
          <select name="wifi-network" id="wifi-network">
            <option value="john" selected="selected">Johns Network</option>
            <option value="sarah">Sarah Network</option>
            <option value="open">Open wifi</option>
            <option value="6HDD-router">6HDD-router</option>
          </select>
          <label for="wifi-pass">Wifi Password</label>
          <input type="password" id="pass" name="password"
            minlength="8">
      </form>

    <nuxt-link to="/box-setup" class="btn btn-primary wizard-button">Next</nuxt-link>

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

