<script>
  export default {
    data() {
      return {
        number: 0
      }
    },
    methods: {
      increase() {
        this.number ++
      },
      decrease() {
        this.number --
      }
    }
  }
</script>

<template>
  <h1>Counter App</h1>
  <h2>{{ number }}</h2>
  <button @click="decrease">-</button>
  <button @click="increase">+</button>
</template>

<style>
  h1 {
    color: blue;
  }
  h2 {
    color: aqua;
  }
</style>
