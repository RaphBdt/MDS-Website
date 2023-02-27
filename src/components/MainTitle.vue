<script setup lang="ts">
defineProps<{
  msg?: string
}>()
</script>
<script lang="ts">
export default {
    setup() {

    }
}
</script>

<template>
    <h1 class="font-extrabold text-[50px] text-center leading-[60px]">{{ msg }}</h1>
</template>

<style scoped>

</style>
