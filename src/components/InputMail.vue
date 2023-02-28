<script lang="ts">
import { defineComponent } from 'vue'
import Button from './Button.vue'


export default defineComponent({
    components: { Button }
})
</script>

<template>
    <form class="w-[550px] mx-auto">   
        <label for="search" class="mb-2 text-sm font-medium text-gray-900 sr-only dark:text-white">Search</label>
        <div class="relative">
            <input type="search" id="search" class="rounded-full mt-16 block w-full p-5 pl-10 text-md text-gray-900 border border-gray-300 bg-gray-50 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500 border-full" placeholder="Entre ton adresse e-mail ici" required>
            <Button class="absolute right-[10px] bottom-[8px]" text="Envoyer" />
        </div>
    </form>
</template>

<style scoped>

</style>