<template>
  <div id="app">
    <TablaLed/>
  </div>
</template>

<script>
import TablaLed from './components/tablaled'

export default {
  name: 'App',
  components: {
    TablaLed
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
