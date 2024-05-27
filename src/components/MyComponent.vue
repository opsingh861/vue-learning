<script setup>

</script>

<template>
    <div>
        <h1 class="global">This is global CSS from MyComponent</h1>
        <h1 class="local">This is local CSS from MyComponent</h1>
        <h1 :class="$style['kabab-case']">This is modular css using kabab case</h1>
        <h1 :class="$style.camleCase">This is modular css using camel case</h1>
        <h1 :class="myStyle.custom">This is modular css using custom module name</h1>
    </div>
</template>

<style>
.global {
    color: red;
}
</style>

<style scoped>
.local {
    color: blue;
}
</style>

<style module>
.kabab-case {
    color: green;
}

.camleCase {
    color: yellow;
}
</style>

<style module="myStyle">
.custom {
    color: purple;
}
</style>