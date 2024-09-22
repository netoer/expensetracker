<template>
    <div>
        <h3>Historial</h3>
        <ul id="list" class="list">
            <li v-for="transaction in transactions" v-bind:key="transaction.id">
                {{ transaction.text }} 
                <span>-${{ transaction-amount }}</span>
                <button class="deleta-btn">X</button>
            </li>
            <button class="delate-btn"></button>
        </ul>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';
const props = defineProps({
    transactions: {
        type: Array,
        required: true,
    }


});
</script>

