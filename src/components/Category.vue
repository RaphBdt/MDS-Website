<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    props: {
        title: String,
        description: String
    },
    setup(props) {
        
    },
})
</script>

<template>
    <div class="bg-white drop-shadow-xl w-[270px] min-h-[250px] px-8 py-6 rounded-[16px]">
        <div class="bg-[#29B7C5] w-[54px] h-[54px] rounded-lg flex items-center justify-center mb-5">
            <img src="../assets/icon-category.svg" alt="">
        </div>
        <h3 class="font-bold text-[20px]">{{ title }}</h3>
        <p class="mb-5">{{ description }}</p>
        <a class="font-bold" href="">Découvrir</a>
    </div>
</template>

<style scoped>

</style>