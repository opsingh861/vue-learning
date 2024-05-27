<script setup>
import { reactive, ref } from 'vue'
const obj = reactive({ count: 0 }) // reactive object, it doesn't support premitive datatypes like string, number, boolean
const count = ref(0) // ref object, it supports premitive datatypes like string, number, boolean

const increment = () => {
    count.value++ // we need to use .value to access the value of ref object
}

const decrement = () => {
    count.value-- // we need to use .value to access the value of ref object
}

</script>

<template>
    <div>
        <!-- <h1>Count: {{ obj.count }}</h1>
        <button @click="obj.count++">Increment</button>
        <button @click="obj.count--">Decrement</button> -->

        <h1>Count: {{ count }}</h1>
        <button @click="increment">Increment</button>
        <button @click="decrement">Decrement</button>

    </div>
</template>