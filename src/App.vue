<template>
  <div id="app">
    <Receiver />
  </div>
</template>

<script>
import Receiver from './components/Receiver'

export default {
  name: 'App',
  components: {
    Receiver
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
