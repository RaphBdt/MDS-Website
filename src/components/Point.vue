<script setup lang="ts">
defineProps<{
  color?: string,
  size?: string
}>()
</script>
<script lang="ts">
export default {
    setup() {
        
    }
}
</script>

<template>
    <div :class="`rounded-full ${color} ${size}`">
        
    </div>
</template>

<style scoped>
    .primary {
        background-color: #29B7C5;
    }

    .secondary {
        background-color: #0F8793;
    }

    .dark {
        background-color: #443A3A;
    }

    .small {
        height: 20px;
        width: 20px;
    }

    .medium {
        height: 28px;
        width: 28px;
    }

    .big {
        height: 40px;
        width: 40px;
    }
</style>
