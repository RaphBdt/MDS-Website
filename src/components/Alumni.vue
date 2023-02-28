<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    props: {
        img: String,
        firstname: String,
        promotion: String,
        description: String,
        date: String,
    },
    setup(props) {
        
    },
    methods: {
        getImageUrl() {
            // This path must be correct for your file
            return new URL(`../assets/${this.img}`, import.meta.url).href
        }
    },
})
</script>

<template>
    <div class="bg-white p-10 rounded-xl drop-shadow-2xl">
        <div class="flex items-center">
            <img class="w-[60px] h-[60px] rounded-xl mr-5" :src="getImageUrl()" alt="">
            <div>
                <p class="font-bold">{{ firstname }}</p>
                <p class="text-[#9D9D9D]">{{ promotion }}</p>
            </div>
        </div>
        <p class="mt-8">{{ description }}</p>
        <p class="font-bold mt-12">{{ date }}</p>
    </div>
</template>

<style scoped>

</style>