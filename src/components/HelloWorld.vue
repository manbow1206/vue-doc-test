<template>
  <ul id="v-for-object" class="demo">
    <li v-for="value in object" :key="value">
      {{value}}
    </li>
  </ul>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      object: {
        title : 'How to do lists in Vue',
        author : 'Jane Doe',
        publisheedAt:'2016-04-10'
      }
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
