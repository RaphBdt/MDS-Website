<script setup lang="ts">
defineProps<{
  text?: string
}>()
</script>
<script lang="ts">
export default {
    setup() {

    }
}
</script>

<template>
    <a class="bg-[#29B7C5] px-6 py-3 text-white rounded-full" href="">{{ text }}</a>
</template>

<style scoped>

</style>
