<template>
    <span class="name">{{userData.name}}</span>
     <span class="handle">{{userData.handle}}</span>
</template>

<script setup>
import {defineProps} from 'vue'
const props = defineProps (["userData"]);
</script>

<style scoped>
</style>