<script lang="ts">
import { defineComponent } from 'vue'
import OtherTitle from './OtherTitles.vue'

export default defineComponent({
    components: { OtherTitle },
    props: {
        title: String,
        description: String
    },
    setup(props) {
        
    },
})
</script>

<template>
    <div id="newsletter-section" class="w-full h-[700px] pt-16">
        <OtherTitle class="text-white text-center w-[600px] mx-auto" type="h2" msg="Entre ton e-mail pour recevoir le programme de l’école" />
        <p class="text-white text-[20px] text-center leading-[26px] mt-10 font-light">Nous t’enverrons le programme complet, et quelqu’un<br /> prendra contact avec toi pour savoir tes besoins</p>
    </div>
</template>

<style scoped>
    #newsletter-section {
        background-image: url('../assets/email.svg');
        background-size: contain;
        background-repeat: no-repeat;
    }
</style>