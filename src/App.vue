<template>
  <div id="app">
    <hello></hello>
    <newtodo></newtodo>
  </div>
</template>

<script>
import Hello from './components/Hello'
import Newtodo from './components/Newtodo.vue'

export default {
  name: 'app',
  components: {
    Hello,
    Newtodo
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
  font-weight: bold;
  background-color: rgba(42, 171, 210, 0.31);
  width: 500px;
  min-height: 150px;
  position: absolute;
  left: 40%;
  border-radius: 5px;
}
</style>
