<template>
<span class="general-header-container">
    <header
      class="sticky flex justify-between items-center w-full pin-t p-4 bg-primary"
    >
      <!--
        We may want the header to disappear when content is scrolled down and reappear when scrolled up
      -->
      <span><i v-on:click="showdrawer = !showdrawer" class="text-4xl material-icons text-white cursor-pointer">menu</i> </span>

      <span>
        <h1 class="text-xl pl-2 text-white font-normal ">
          <slot name="header-title">title goes here</slot>
        </h1>
        </span>
      <span><i class="material-icons text-white cursor-pointer">more_vert</i></span>
    </header>
    <transition name="slide">
      <span v-show="showdrawer" class="general-nav-drawer min-h-screen bg-white shadow-lg w-64 z-10 fixed inline-block p-4">
        <img class="center h-32 w-32 block pb-4 border-b-2" src="~/assets/images/Circular-Image-with-Icon.png">
        <nuxt-link to="/summary" class="block">Summary</nuxt-link>
        <nuxt-link to="/history" class="block">History</nuxt-link>
        <nuxt-link to="/settings" class="block">Settings</nuxt-link>

      </span>
    </transition>

</span>
</template>

<style>
.slide-enter-active, .slide-leave-active {
  transition: all .3s ease-in-out;
}

.slide-enter, .slide-leave-to
/* .slide-leave-active below version 2.1.8 */ {
  transform: translateX(-256px);
}
</style>


<script>

export default {

    data() {
      return {
      showdrawer: true
    }
  }

}
</script>

