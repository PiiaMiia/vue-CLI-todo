<template>
  <div id="get-todo" class="container">
    <span id="title">Vue.js todo list</span>
    <br>
    <input class="form-control"
           :value="newTodo"
           @change="getTodo"
           placeholder="Add new task here">
    <button class="btn btn-primary" @click="addTodo">Add Todo</button>
  </div>
</template>
<script>
  export default{
    methods: {
      getTodo (e) {
        this.$store.dispatch('getTodo', e.target.value)
      },
      addTodo () {
        this.$store.dispatch('addTodo')
        this.$store.dispatch('clearTodo')
      }
    },
    computed: {
      newTodo () {
        return this.$store.getters.newTodo
      }
    }
  }
</script>

<style>
  #get-todo {
    width: 400px;
    margin-left: 25px;
    margin-top: 25px;
  }
  #title {
    text-align: right;
  }
</style>
