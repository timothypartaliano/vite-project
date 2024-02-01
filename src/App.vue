<script>
  export default {
    data() {
      return {
        title: 'Hello World',
        subtitle: 'Hello Vue'
      }
    }
  }
</script>

<template>
  <h1>{{ title }}</h1>
    <br>
  <h2>{{ subtitle }}</h2>
</template>

<style>
  h1 {
    color: blue;
  }
  h2 {
    color: aqua;
  }
</style>
