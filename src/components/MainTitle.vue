<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    props: {
        msg: String
    },
    setup(props) {

    },
})
</script>

<template>
    <h1 class="font-extrabold text-[50px] text-center leading-[60px]">{{ msg }}</h1>
</template>

<style scoped>

</style>