<template>
  <div class="iteration">

    <h1>5 Bonus | Change the background color of an element when pressing a button</h1>
    <hr>

    <div class="box" :class="colorBackground ? 'color-green' : 'color-red'">
      <button @click="changeColorOrder">Click me to change mood</button>  
    </div>

  </div>
</template>


<script setup>
import {ref} from "vue";

const colorBackground = ref(true);

function changeColorOrder(){
  colorBackground.value = !colorBackground.value;
};

</script>


<style scoped>
.box {
  width: 100%;
  height: 20rem;
  margin: 1rem 0;
  display: flex;
  align-items: center;
  justify-content: center;
}
.color-green {
  background-color: greenyellow;
}
.color-red {
  background-color:  red;
}
button {
  padding: 2rem;
}
.iteration {
  min-height: 50vh;
  display: block;
  align-items:center;
}
h1 {
  margin-bottom: 3rem;
}

  
</style>
