<!-- Composition API -->
<script setup>
import {ref} from "vue"

const count = ref(0);
const text = ref(0);

const increment = () => {
  count.value++;
}

const updateCount = (e) => {
  count.value = Number(e.target.value);
}
</script>

<template>
  <h1>Count: {{ count }}</h1>
  <button @click="increment">+1</button>
  <!--  Плохой пример кода -->
  <input @input="updateCount">
  <br>
  <!-- Хороший пример. Из документации  -->
  <h1>Text: {{ text }}</h1>
  <input
      :value="text"
      @input="event => text = event.target.value">
</template>


<style scoped></style>
