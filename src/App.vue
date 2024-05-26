<script setup> // we need to add setup so that we can use the script tag in the single file component
const msg = "hello world";
</script>

<template>
  <h1>hello world</h1>
  <h1>String interpolation: {{ msg }} </h1>
</template>