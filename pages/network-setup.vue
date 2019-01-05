<template>
  <div class="nuxt-holding-element">

    <main class="min-h-screen flex flex-col mt-12 items-center">

      <h1>Network Setup</h1>
      <div class="network_icon mb-4">
        <svg width="113" height="113" viewBox="0 0 113 113" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M87.1464 81.6036L87.2929 81.75H87.5H112V112H81.75V93.4375V93.2375L81.6121 93.0927L56.6121 66.8427L56.25 66.4625L55.8879 66.8427L30.8879 93.0927L30.75 93.2375V93.4375V112H0.5V81.75H25H25.2071L25.3536 81.6036L50.3536 56.6036L50.5 56.4571V56.25V36.375V36.0243L50.1702 35.9049C43.1063 33.3473 38 26.6522 38 18.75C38 8.65114 46.1511 0.5 56.25 0.5C66.3489 0.5 74.5 8.65114 74.5 18.75C74.5 26.6522 69.3937 33.3473 62.3298 35.9049L62 36.0243V36.375V56.25V56.4571L62.1464 56.6036L87.1464 81.6036Z" stroke="#607D8B"/>
        </svg>
      </div>
      <p class="mx-8 mt-4 max-w-xs">Make sure your iMyner box is connected via an Ethernet cable to your Internet connection</p>

    <nuxt-link to="/wifi-setup" class="btn btn-primary wizard-button">Next</nuxt-link>

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

