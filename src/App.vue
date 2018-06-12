<template>
  <div id="app">
    <kanban msg="Hi"/>
  </div>
</template>

<script>
import Kanban from './components/Kanban.vue'

export default {
  name: 'app',
  components: {
    Kanban
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
