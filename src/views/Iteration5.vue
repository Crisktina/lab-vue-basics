<template>
  <div class="iteration">

    <h1>5 Bonus | Change the background color of an element when pressing a button</h1>
<hr>

<button @click="changeColor()">Change background color</button>

 <div :class="box1">
    <h3 v-if= "string === true">You can do it!</h3>
    <h3 v-else>Better try again</h3>
</div>

  </div>
</template>


<script setup>
import {ref} from "vue";


const string = ref(true);

function changeColor(){
    
    alert('You clicked on!')
}

let box1 = ref("border");
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
.border {
    border: 3px solid greenyellow;
    width: 100%;
    height: 50px;
    margin: 10px 0;
    display: flex;
    align-items: center;
    justify-content: center;

}
  button {
    padding: 2rem;
    width: 100%;
  }
</style>
