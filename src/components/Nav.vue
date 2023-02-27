<script setup lang="ts">
import Button from './Button.vue'
</script>
<script lang="ts">
export default {
    setup() {

    }
}
</script>

<template>
    <nav>
        <div class="container mx-auto">
            <div class="flex justify-between items-center">
                <a href="https://vuejs.org/" target="_blank">
                    <img src="../assets/logo-mds.png" class="logo vue w-[131px]" alt="Logo MDS" />
                </a>
                <div>
                    <a class="text-[#07052F] font-bold mx-3">Accueil</a>
                    <a class="text-[#A5A5A5] font-bold mx-3">Les programmes</a>
                    <a class="text-[#A5A5A5] font-bold mx-3">Notre blog</a>
                </div>
                <Button text="M'inscrire" />
            </div>
        </div>
    </nav>
</template>

<style scoped>

</style>
