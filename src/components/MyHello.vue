<script setup>
defineProps({
  title: String,
  price: Number,
  isAdded: Boolean,
});
</script>

<template>
  <div class="product m-2.5">
    <h2 class="text-amber-600">Товар: {{ title }}</h2>
    <h3 class="font-bold underline">Цена: {{ price }}р.</h3>
    <h3>Добавлен в корзину: {{ isAdded ? "Да" : "Нет" }}</h3>
    <slot/>  <!-- slot => аналог children из React  -->
  </div>

</template>

<style scoped>
.product {
  display: flex;
  flex-direction: column;
  border: 1px solid blue;
  padding: 10px;
  margin-bottom: 10px;
}
</style>
