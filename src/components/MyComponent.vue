<script setup>
import { reactive } from 'vue'
const obj = reactive({ count: 0 }) // reactive object, it doesn't support premitive datatypes like string, number, boolean
</script>

<template>
    <div>
        <h1>Count: {{ obj.count }}</h1>
        <button @click="obj.count++">Increment</button>
        <button @click="obj.count--">Decrement</button>
    </div>
</template>