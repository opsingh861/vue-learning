<script setup>// we need to add setup so that we can use the script tag in the single file component
const msg = "hello world";
const imgSrc = "https://vuejs.org/images/logo.png";
const title = "Attribute binding";
const height = 500;
const width = 500;
</script>

<template>
  <h1>Attribute binding</h1>
  <!-- <img :src="imgSrc" alt="title" height="500" width="500" /> if we just want to hard code the value we can just give the value directly -->
  <!-- <img :src="imgSrc" alt="title" :height="height" :width="width" /> -->
  <img v-bind:src="imgSrc" alt="title" v-bind:height="height" v-bind:width="width" />
</template>