<template>
<img :src="image" class="profile"/>
</template>

<script setup>
import {defineProps} from 'vue'
const props = defineProps (["image"]);
</script>

<style scoped>
</style>