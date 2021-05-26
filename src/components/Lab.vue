<template>
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
  `,
    data(){
        return {
          postFontSize: 1
        }
    }
}
</script>

<style scoped>
div{
    border: 2px solid teal
}
h1{
    color: teal
}
p{
    color:rgb(27, 77, 77)
}
</style>
