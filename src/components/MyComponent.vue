<script setup>
const clickHandler = () => {
    alert('clicked')
}
const clickHandlerParam = (data) => {
    alert(data)
}
const submitHandler = (event) => {
    event.preventDefault()
    alert('submitted')
}
</script>

<template>
    <h1>Events</h1>
    <button v-on:click="clickHandler">Click here</button>
    <button @click="clickHandler">Click here</button>
    <button @click="clickHandlerParam('Aditya')">Click here</button>
    <form @submit="submitHandler">
        <input type="text" placeholder="Please enter your name" />
        <input type="text" placeholder="Please enter your email" />
        <button type="submit">Submit</button>
    </form>

</template>