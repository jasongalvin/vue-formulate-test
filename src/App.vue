<template>
  <div id="app">
    <register-test />
  </div>
</template>

<script>
import RegisterTest from './components/RegisterTest.vue'

export default {
  name: 'App',
  components: {
    RegisterTest,
  }
}
</script>

<style>
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
}
</style>
