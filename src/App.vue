<template>
  <div id="app" class="container">
    <GetTodo></GetTodo>
    <CurrentTodos></CurrentTodos>
  </div>
</template>

<script>
  import GetTodo from './components/GetTodo.vue'
  import CurrentTodos from './components/CurrentTodos.vue'
  export default {
    components: {
      GetTodo,
      CurrentTodos
    }

  }
</script>

<style>
  #app {
    background-color: rgba(42, 171, 210, 0.31);
    width: 500px;
    min-height: 150px;
    position: fixed;
    left: 50%;
    top: 25px;
    margin-left: -250px;
    border-radius: 5px;
  }
</style>
