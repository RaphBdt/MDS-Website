<script setup lang="ts">
defineProps<{
  type?: string,
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
    <h2 v-if="type === 'h2'" class="font-extrabold text-[50px] text-center leading-[60px]">{{ msg }}</h2>
    <h3 v-if="type === 'h3'" class="font-bold text-[18px] text-center uppercase text-[#29B7C5]">{{ msg }}</h3>
</template>

<style scoped>

</style>