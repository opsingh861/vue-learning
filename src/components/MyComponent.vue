<script setup>
import { ref, computed } from 'vue'

const count = ref(0)

const square = computed(() => count.value ** 2) // we need to give a function to computed

function increment() {
    count.value++
}

function decrement() {
    count.value--
}
</script>

<template>
    <div>
        <!-- <h1>Count: {{ obj.count }}</h1>
        <button @click="obj.count++">Increment</button>
        <button @click="obj.count--">Decrement</button> -->

        <h1>Count: {{ count }}</h1>
        <h1>Square: {{ square }}</h1>
        <button @click="increment">Increment</button>
        <button @click="decrement">Decrement</button>

    </div>
</template>