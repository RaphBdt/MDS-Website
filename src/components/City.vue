<script lang="ts">
import { defineComponent } from 'vue'
import Container from './Container.vue'

export default defineComponent({
    components: { Container }
})
</script>

<template>
    <Container>
        <div class="flex items-end justify-center">
            <div class="mx-8 flex flex-col items-center">
                <img class="w-[110px] h-auto" src="../assets/ville1.png" alt="">
                <p class="mt-5 uppercase font-bold text-[#686868]">2000 étudiants</p>
            </div>
            <div class="mx-8 flex flex-col items-center">
                <img class="w-[140px] h-auto" src="../assets/ville2.png" alt="">
                <p class="mt-5 uppercase font-bold text-[#686868]">2000 étudiants</p>
            </div>
            <div class="mx-8 flex flex-col items-center">
                <img class="w-[150px] h-auto" src="../assets/ville3.png" alt="">
                <p class="mt-7 uppercase font-bold text-[#686868]">2000 étudiants</p>
            </div>
            <div class="mx-8 flex flex-col items-center">
                <img class="w-[120px] h-auto" src="../assets/ville4.png" alt="">
                <p class="mt-5 uppercase font-bold text-[#686868]">2000 étudiants</p>
            </div>
        </div>
    </Container>
</template>

<style scoped>

</style>