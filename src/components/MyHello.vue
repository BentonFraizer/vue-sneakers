<script setup>
defineProps({
  title: String,
  price: Number,
  isAdded: Boolean,
});
</script>

<template>
  <div class="product">
    <h2>Товар: {{ title }}</h2>
    <h3>Цена: {{ price }}р.</h3>
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
