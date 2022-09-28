<template>
  <div class="iteration">
    <h1>2 | Display the result of a Javascript operation in a component's HTML</h1>
    <hr>
    <h2>Part 1 | This string has to be returned by a function:</h2>
    <p>{{ 2 + 2 }}</p>
    <h2>Part 2 | This string has to be returned by a function:</h2>
    <input type="text" v-model="number1">
    <span>+</span>
    <input type="text" v-model="number2">
    <div>Result: {{result}}</div>
  </div>
</template>


<script setup>
import {ref, computed} from "vue";

const number1 = ref("0");
const number2 = ref("0");

const result = computed(()=>{
  return parseInt(number1.value) + parseInt(number2.value);
})
  
</script>


<style>

  .iteration {
    min-height: 50vh;
    display: block;
    align-items:center;
  }
  h1 {
    margin-bottom: 3rem;
  }

</style>
