<template>
    <h1>Tu saldo es:</h1> 
    <h2 id="balance">${{total}}</h2>
</template>
<script setup>
import { defineProps } from 'vue';
const props = defineProps({
    total: {
        type: Number,
        Required: true
    }
})
</script>