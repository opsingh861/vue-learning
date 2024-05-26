<script setup>// we need to add setup so that we can use the script tag in the single file component
const imageInfo ={
  src: 'https://vuejs.org/images/logo.png',
  alt: 'Vue.js Logo',
  width: '100',
  height: '100'

}
</script>

<template>
  <h1>Dynamic attributes</h1>
  <img :="imageInfo" />
</template>