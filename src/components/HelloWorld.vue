<template>
<ul id="example1">
  <li v-for="todo in todos" v-if="!todo.isComplete">
    {{ todo }}
  </li>
</ul>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      numbers: [1,2,3,4,5,6]
    }
  },
  computed: {
    evenNumbers: function() {
      return this.numbers.filter(function (number) {
        return number % 2 === 0
      })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
