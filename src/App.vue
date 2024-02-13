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
      increment(event, input) {
        this.number += input
        this.input = 0
        event.preventDefault()
    }
  },
  components: { CounterApp, FormApp }
}
</script>

<template>
  <h1>Counter App</h1>
  <CounterApp :number="number" title="Component App"></CounterApp>
  
  <FormApp @increment="increment"></FormApp>

</template>

<style>
  h1 {
    color: blue;
  }
  h2 {
    color: aqua;
  }
</style>
