<script>
export default {
  data() {
    return {
      count: 0,
    }
  },
  methods: {
    increment() {
      this.count++
    }
  }
}
</script>

<template>
  <h1>Count: {{ count }}</h1>
  <button @click="increment">+1</button>
</template>


<style scoped></style>
