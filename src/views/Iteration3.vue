<template>
  <div class="iteration">
    <MyComponent />
  </div>
</template>

<script setup>
import MyComponent from '../components/MyComponent.vue'
import { ref } from "vue";

</script>

<style>
@media (min-width: 1024px) {
  .iteration {
    min-height: 50vh;
    display: block;
    align-items:center;
  }
}
</style>
