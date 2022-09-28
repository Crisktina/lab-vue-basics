<template>
 
    <div :class="box1">
        <h2 v-if= "mood">You can do it!</h2>
        <h2 v-else>Better try again</h2>
    </div>
    <h2 v-show= "mood2">You got it girl!</h2>
</template>

<script setup>
import { ref } from "vue";
let box1 = ref("border");

const mood = ref(true);
const mood2 = ref(true);

</script>

<style>
.border {
    border: 3px solid greenyellow;
    width: 100%;
    height: 50px;
    margin: 10px 0;
    display: flex;
    align-items: center;
    justify-content: center;

}

</style>
