<template>
  <div class="nuxt-holding-element">
    <main class="min-h-screen flex flex-col mt-12 items-center">
      <h1>Welcome</h1>
      <div class="my-4">
        <!-- TODO: replace with SVG version once we find out what didn't translate -->
        <img class="center" src="~/assets/images/tracky-tracky-logo192.png">
      </div>
      <sub class="m-2">Tracky Tracky Logo</sub>

      <nuxt-link to="/network-setup" class="btn wizard-button">Start</nuxt-link>
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

