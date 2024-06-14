<template>
  <div id="app">
    <TeListUsers/>
  </div>
</template>

<script>
import TeListUsers from './components/TeListUsers.vue'

export default {
  name: 'App',
  components: {
    TeListUsers
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
