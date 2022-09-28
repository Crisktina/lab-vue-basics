<template>
  <div class="iteration">
    <h1>3 | Show an element only if a particular property is set to true</h1>
    <hr>
    <MyComponent />
  </div>
</template>

<script setup>
import MyComponent from '../components/MyComponent.vue'
import { ref } from "vue";

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
