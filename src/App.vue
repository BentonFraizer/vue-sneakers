<script setup>
import MyHello from "@/components/MyHello.vue";
</script>

<template>
  <MyHello title="Кроссовки Puma" :price="19500" is-added>
    <button>Добавить</button>
  </MyHello>
  <MyHello isAdded>
    <h5>Нет в наличии</h5>
  </MyHello>
  <MyHello isAdded>
    <MyHello>
      <h5>Нет в наличии</h5>
    </MyHello>
  </MyHello>
  <MyHello :isAdded="false"/>
</template>

<style scoped>
</style>
