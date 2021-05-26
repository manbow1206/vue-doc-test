<template>
  <div id="blog-posts-events-demo">
  <div :style="{ fontSize: postFontSize + 'em' }">
    <Lab
      v-for="post in posts"
      v-bind:key="post.id"
      v-bind:post="post"
      v-on:enlarge-text="postFontSize += 0.1"
    ></Lab>
  </div>
</div>
</template>

<script>
import Lab from './components/Lab.vue'

export default {
  data: {
    postFontSize: 1
  },
  components: {
    Lab
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
