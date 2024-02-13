<script>
import CounterApp from './components/CounterApp.vue'

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
  },
  components: { CounterApp }
}
</script>

<template>
  <h1>Counter App</h1>
  <CounterApp :number="number" title="Component App"></CounterApp>
  
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
