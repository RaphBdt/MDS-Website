<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    props: {
        direction: String
    },
    setup(props) {

    },
})
</script>

<template>
    <div>
        <div v-if="direction == 'left'" class="rounded-full w-[50px] h-[50px] border-2 border-[#29B7C5] flex items-center justify-center">
            <img class="w-[25px] h-[25px]" src="../assets/left-arrow.svg" alt="">
        </div>
        <div v-if="direction == 'right'" class="rounded-full w-[50px] h-[50px] bg-[#29B7C5] flex items-center justify-center">
            <img class="w-[25px] h-[25px]" src="../assets/right-arrow.svg" alt="">
        </div>
    </div>
</template>

<style scoped>

</style>
