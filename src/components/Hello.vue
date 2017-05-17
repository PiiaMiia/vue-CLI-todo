<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Vue to-do app'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .hello {
    text-align: left;
    margin-left: 15px;
  }

  h1, h2 {
    font-weight: normal;
  }

  a {
    color: #42b983;
  }
</style>
