<template>
  <div class="newtodo">
    <h3 id="instruction">Insert a new thing: <input v-model="todo"></h3>
    <p>
      Your new task is:
      <br>
      <br>
      <span id="newtodo">{{ todo }}</span>
      <br>
      <br>
      Hit submit to confirm.
    </p>
    <button id="submit">SUBMIT</button>
  </div>
</template>

<script>
  export default {
    name: 'newtodo',
    data () {
      return {
        todo: 'Brush your hair!'
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
  }

  h1, h2, h3, p, span {
    color: #165f7b;
  }

  a {
    color: #48b8ff;
  }

  #instruction {
    text-align: left;
    margin-left: 15px;
  }

  #submit {
    background-color: rgba(31, 151, 192, 0.5);
    border-color: #165f7b;
    color: #165f7b;
    position: relative;
    left: 200px;
    margin-bottom: 15px;

  }

  #newtodo {
    color: rgba(42, 172, 221, 0.65);
    margin-top: 15px;
  }
</style>
