<template>
 <div class="nuxt-holding-element">

  <GeneralHeader>
   <span slot="header-title">title 2</span>
  </GeneralHeader>

  <section class="container mx-auto border border-black p-4 m-4">
    <div>
      <logo/>
      <h1 class="title">
        Multi Layout
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
