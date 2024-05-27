<script setup>// we need to add setup so that we can use the script tag in the single file component
import MyComponent from './components/MyComponent.vue'
</script>

<template>
  <div>
    <MyComponent />
    <h1 class="global">This is global css from App component</h1>
    <h1 class="local">This is local css from App component</h1>  <!-- this will not work because the css is local to MyComponent.vue -->
  </div>
</template>