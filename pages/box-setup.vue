<template>
  <div class="nuxt-holding-element">

    <main class="min-h-screen flex flex-col mt-12 items-center">

      <h1>Setup Box</h1>
      <div class="router_icon mb-4">
        <svg width="113" height="113" viewBox="0 0 113 113" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M87 62.5V63H87.5H100C106.599 63 112 68.4011 112 75V100C112 106.599 106.599 112 100 112H12.5C5.90114 112 0.5 106.599 0.5 100V75C0.5 68.4011 5.90114 63 12.5 63H75H75.5V62.5V38H87V62.5ZM100 100.5H100.5V100V75V74.5H100H12.5H12V75V100V100.5H12.5H100ZM107.483 17.4348C99.9575 10.6859 90.6113 7 81.25 7C71.8887 7 62.5425 10.6859 55.0169 17.4348L50.709 13.1269C59.3121 4.70628 70.2827 0.5 81.25 0.5C92.2173 0.5 103.188 4.70628 111.791 13.1269L107.483 17.4348ZM65.629 27.4219L61.335 23.1279C66.8277 17.8144 74.0445 14.875 81.25 14.875C88.4555 14.875 95.6723 17.8144 101.165 23.1279L96.871 27.4219C92.4422 23.1894 86.8357 21.375 81.25 21.375C75.6643 21.375 70.0578 23.1894 65.629 27.4219ZM19.25 81.75H30.75V93.25H19.25V81.75ZM41.125 81.75H52.625V93.25H41.125V81.75ZM63 81.75H74.5V93.25H63V81.75Z" stroke="#607D8B"/>
        </svg>
      </div>
      <h3 class="my-4">Boxes Available</h3>
      <h4>imyn_node_63</h4>

    <button class="btn-tertiary my-4">Rescan</button>

    <nuxt-link to="/location-setup" class="btn btn-primary wizard-button">Next</nuxt-link>

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

