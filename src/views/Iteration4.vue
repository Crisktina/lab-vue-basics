<template>
  <div class="iteration">
    
    <h1>Iteration 4 | Display a list of elements that are stored inside a component</h1>
    <hr>
    <div v-for="(post, index) in posts" :key="index">
        <h3>{{ index }} - {{ post.title }} - {{ post.description }}</h3>
        <p v-for="(post, index) in posts.content" :key="index">
          {{ index }} - {{ content }}
        </p>
    </div>

  </div>
</template>


<script setup>
import { ref } from "vue";

const posts = ref(
    [{title: "Croquetas", description: "Spain", content: ["milk", "flour"]},
    {title: "Berengenas rellenas", description: "Spain", content: ["eggplant", "chesse"]},
    {title: "Gazpacho", description: "Spain", content: ["tomatoe", "olive oil"]},
    {title: "Pollo tika masala", description: "Índia", content: ["curry", "chicken"]},
    {title: "Canelones de setas", description: "Italia", content: ["mushroms", "chesse"]},
    {title: "Ensalada de queso de cabra", description: "Francia", content: ["letuce", "goat chesse"]},
    {title: "Tarta de queso", description: "Spain", content: ["chesse", "baking powder"]},
    {title: "Sushi", description: "Japón", content: ["rice", "salmon"]}]
);
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
