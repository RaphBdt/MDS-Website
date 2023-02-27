<script setup lang="ts">
import Point from './Point.vue'
</script>

<script lang="ts">
export default {
    setup() {

    }
}
</script>

<template>
    <div class="container flex justify-center relative">
        <Point class="absolute left-[270px] -top-[80px] point1" color="primary" size="medium" />
        <Point class="absolute left-[100px] top-[60px]" color="dark" size="small" />
        <Point class="absolute left-[290px] top-[300px]" color="secondary" size="medium" />
        <Point class="absolute left-[760px] top-[0px]" color="dark" size="small" />
        <Point class="absolute right-[280px] -top-[80px]" color="primary" size="medium" />
        <Point class="absolute right-[170px] top-[170px]" color="secondary" size="big" />
        <Point class="absolute right-[400px] top-[300px]" color="primary" size="small" />

        <div class="flex mx-auto">
            <img class="w-[160px] h-[250px] mx-3 object-cover" src="../assets/profile1.png" alt="">
            <img class="w-[160px] h-[250px] mx-3 mt-20 object-cover" src="../assets/profile2.png" alt="">
            <img class="w-[160px] h-[250px] mx-3 mt-20 object-cover" src="../assets/profile3.png" alt="">
            <img class="w-[160px] h-[250px] mx-3 object-cover" src="../assets/profile4.png" alt="">
        </div>
    </div>
</template>

<style scoped>

</style>
