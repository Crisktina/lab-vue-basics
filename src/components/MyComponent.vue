<template>
 
   <div>
    <h1>Iteration 3 | Show an element only if a particular property is set to true</h1>
    <div :class="box1">
        <h2 v-if= "mood === true">Mood: You can do it!</h2>
        <h2 v-else>Mood: Better try again</h2>
    </div>
   </div>

</template>

<script setup>
import { ref } from "vue";
let box1 = ref("border");

const mood = ref(true);

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
