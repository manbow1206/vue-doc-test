<template>
  <!-- <input v-model.lazy="msg"> -->
  <input v-model.number="age" type="number">
  <!-- <input v-model.trim="msg""> -->
</template>

<script>
export default {
   data: {
    checkedNames: []
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
