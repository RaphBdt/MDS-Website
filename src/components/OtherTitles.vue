<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    props: {
        type: String,
        msg: String
    },
    setup(props) {
        
    },
})
</script>

<template>
    <div>
        <h2 v-if="type === 'h2'" class="font-extrabold text-[38px] text-center leading-[50px]">{{ msg }}</h2>
        <h3 v-if="type === 'h3'" class="font-bold text-[18px] text-center uppercase text-[#29B7C5]">{{ msg }}</h3>
    </div>
</template>

<style scoped>

</style>