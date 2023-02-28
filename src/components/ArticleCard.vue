<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    props: {
        img: String,
        date: String,
        title: String
    },
    setup(props) {
        
    },
    methods: {
        getImageUrl() {
            // This path must be correct for your file
            return new URL(`../assets/${this.img}`, import.meta.url).href
        }
    },
    mounted() {
        console.log(this.getImageUrl);
    }
})
</script>

<template>
    <div class="bg-white rounded-xl p-8 w-[270px] min-h-[250px]">
        <img class="w-full h-[180px] object-cover rounded-xl" :src="getImageUrl()" alt="">
        <p class="my-5">Posté le {{ date }}</p>
        <h3 class="font-bold">{{ title }}</h3>
    </div>
</template>

<style scoped>

</style>