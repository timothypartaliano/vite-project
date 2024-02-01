<script>
  export default {
    data() {
      return {
        number: 0,
        input: 0
      }
    },
    methods: {
      increment(event) {
        this.number += this.input
        this.input = 0
        event.preventDefault()
      }
    }
  }
</script>

<template>
  <h1>Counter App</h1>
  <h2>{{ number }}</h2>

  <form @submit="increment">
    <input type="number" v-model="input">
    <input type="submit">
  </form>
  
</template>

<style>
  h1 {
    color: blue;
  }
  h2 {
    color: aqua;
  }
</style>
