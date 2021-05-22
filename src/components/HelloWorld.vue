<template>
    <div id="app">
      <input type="text" v-on:keyup.enter="alert">
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      name: 'vue.js'
    }
  },
  computed: {
    say: function(say) {
      alert(say)
    }
  },
  methods: {
    alert() {
      alert("アラート！")
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
