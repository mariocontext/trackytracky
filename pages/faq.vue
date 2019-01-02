<template>
  <section class="container mx-auto border border-black p-4 m-4">
    <div>
      <logo/>
      <h1 class="title">
        FAQ
      </h1>
      <h2 class="subtitle text-orange">
        some FAQ text goes here
      </h2>
      <button class="my-btn">transition test</button>
      <testcompo>
        <div slot="firsty">hello from instance 1</div>
      </testcompo>
      <testcompo>
        <div slot="firsty">goodbye from instance 2</div>
        <div slot="secondy">bye bye</div>
      </testcompo>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green">Documentation</a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey">GitHub</a>
        <nuxt-link to="/" class="text-orange">Home page</nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Testcompo from '~/components/Testcompo.vue'

export default {
  components: {
    Logo,
    Testcompo
  }
}
</script>

<style>

/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

.my-btn {
   @apply p-4 my-2 bg-purple rounded;
}

.my-btn:hover {
  background-color: green;
}

.links {
  @apply text-center;
}
</style>
