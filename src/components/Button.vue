<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    props: {
        text: String
    },
    setup(props) {

    },
})
</script>

<template>
    <a class="bg-[#29B7C5] px-6 py-3 text-white rounded-full" href="">{{ text }}</a>
</template>

<style scoped>

</style>
