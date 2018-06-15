<template>
  <div id="app">
    <h1>Hello world</h1>
    <counter></counter>
    <counter></counter>
  </div>
</template>

<script>
  import Counter from './Counter'
export default {
  components: {
      Counter
  },
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="scss">
</style>
