<template>
  <div class="TestComp">
    <div class="text-green my-special-border">
      hello worldoo 
    </div>
    <div>
      <p class="text-red" >
        <slot name="firsty">default firsty</slot>
      </p>
    </div>
    <div>
      <p class="text-blue-light">
        <slot name="secondy">default secondy</slot>
      </p>
    </div>
  </div>
</template>

<style>

</style>
