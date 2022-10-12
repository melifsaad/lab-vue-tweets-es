<template>
    <span class="timeStamp">{{timeStamp}}</span>
</template>

<script setup>
import {defineProps} from 'vue'
const props = defineProps (["timeStamp"]);
</script>

<style scoped>
</style>