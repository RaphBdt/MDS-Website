<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    props: {
        numberOfStudents: String,
        imageFile: String
    },
    setup(props) {

    },
})
</script>

<template>
    <div>
        <img class="w-[200px] h-auto" src="./assets/ville1.png" alt="">
        <p class="uppercase font-bold text-[#686868]">{{ numberOfStudents }} étudiants</p>
    </div>
</template>

<style scoped>

</style>