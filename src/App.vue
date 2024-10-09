<script setup>
 import MyHello from "@/components/MyHello.vue";
</script>

<template>
  <MyHello title="Кроссовки Puma" :price="19500" is-added />
  <MyHello isAdded />
  <MyHello :isAdded="false"/>
</template>

<style scoped>
</style>
