<template>
    <header
      class="sticky flex justify-between items-center w-full pin-t p-4 bg-primary"
    >
      <!--
        We may want the header to disappear when content is scrolled down and reappear when scrolled up
      -->
      <span> <i class="text-4xl material-icons text-white">menu</i> </span>
      <span>
        <h1 class="text-xl pl-2 text-white font-normal ">
          <slot name="header-title">title goes here</slot>
        </h1>
        </span>
      <span><i class="material-icons text-white">more_vert</i></span>
    </header>
</template>
