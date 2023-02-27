<script setup lang="ts">
import Nav from './components/Nav.vue'
import MainTitle from './components/MainTitle.vue'
import Button from './components/Button.vue'
</script>

<template>
  <Nav class="my-14" />
  <MainTitle class="w-[600px] mx-auto mt-20" msg="La meilleure école des métiers du digital" />
  <div class="flex justify-center">
    <Button class="mx-auto mt-8" text="Appelez-nous" />
  </div>
</template>

<style scoped>

</style>
