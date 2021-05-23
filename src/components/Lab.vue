<template>
    <div>
        <h1>{{ propData }}</h1>
        <p>{{ text }}</p>
    </div>
</template>

<script>
export default {
  props: ['post'],
  template: `
    <div class="blog-post">
      <h3>{{ post.title }}</h3>
      <button v-on:click="$emit('enlarge-text')">
        Enlarge text
      </button>
      <div v-html="post.content"></div>
    </div>
  `
}
</script>

<style scoped>
div{
    border: 2px solid
}
h1{
    color: teal
}
p{
    color:rgb(27, 77, 77)
}
</style>
