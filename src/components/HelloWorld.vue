<template v-if="OK">
  <div v-if="type === 'A'">
    A
  </div>
  <div v-else-if="type === 'B'">
    B
  </div>
  <div v-else-if="type === 'C'">
    C
  </div>
  <div v-else>
    Not A/B/C
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      styleObject: {
        color: 'red',
        fontSize: '13px'
      },
    }
  },
  computed: {
    classObject: function() {
      return {
        active: this.isActive && !this.error,
        'test-danger': this.error && this.error.type === 'fatal'
      }
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
