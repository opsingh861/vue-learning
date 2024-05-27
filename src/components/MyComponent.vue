<!-- <template>
    <div>
        using v-if conditionally remove the element from dom itself
        <h1 v-if="colour === 'black'">Black</h1>
        <h1 style="color: red;" v-else-if="colour === 'red'">Red</h1>
        <h1 style="color: blue;" v-else>Blue</h1>
        <button @click="changeColour">Change Colour</button>
    </div>
</template> -->


<template>
    <div>
        using v-show conditionally hide the element using display none property but element still exists in dom
        <h1 v-show="colour === 'black'">Black</h1>
        <h1 style="color: red;" v-show="colour === 'red'">Red</h1>
        <h1 style="color: blue;" v-show="colour === 'blue'">Blue</h1>
        <button @click="changeColour">Change Colour</button>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const colour = ref("black")

const changeColour = () => {
    if (colour.value === 'black') {
        colour.value = 'red'
    } else if (colour.value === 'red') {
        colour.value = 'blue'
    } else {
        colour.value = 'black'
    }
}
</script>
