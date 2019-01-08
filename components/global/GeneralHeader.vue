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
        <img class="center block pb-4" src="~/assets/images/Circular-Image-with-Icon.png" width="60" height="60">
        <div class="nav-listing flex flex-col flex-start border-t-2 pt-4 w-full">
          <nuxt-link to="/summary" class="text-black font-semibold no-underline py-4">
            <span class="material-icons relative" style="top:5px">stars</span>
            Summary
          </nuxt-link>
          <nuxt-link to="/history" class="text-black font-semibold no-underline py-4">
            <span class="material-icons relative" style="top:5px">access_time</span>
            History
          </nuxt-link>
          <nuxt-link to="/settings" class="text-black font-semibold no-underline py-4">
            <span class="material-icons relative" style="top:5px">settings</span>
            Settings
          </nuxt-link>
        </div>
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
      showdrawer: false
    }
  }

}
</script>

