<script setup>
import { ref } from 'vue'
</script>

<template>
    <div class="test">
        hello world2
    </div>
    <div class="hello-world">
        hello world
    </div>
</template>

<style>
.hello-world{
    background-color: red;
    position: relative;
    /* width: 50%;
    height: 50vh;
    top: 50%;
    left: 50%;
    transform: translate(-50%, 50%); */
    right: 60px;
}
.test{
    background-color: blue;
    position: absolute;
    width: 100%;
    height: 100%;
}
</style>