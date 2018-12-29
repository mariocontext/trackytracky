<template>
  <section class="container mx-auto border border-black p-4 m-4">
    <div>
      <logo/>
      <h1 class="title">
        nuxtclitest
      </h1>
      <h2 class="subtitle text-orange">
        test of nuxt with tailwind universal app chosen as opposed to SPA
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green">Documentation</a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey">GitHub</a>
          <nuxt-link class="text-orange" to="/faq">FAQ</nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>

/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

.links {
  @apply text-center;
}
</style>
