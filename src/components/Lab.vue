<template>
  <div class="container">
    <span>
      <slot v-bind:user="user">
        {{ user.lastName }}
      </slot>
    </span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        lastName: 'テスト'
      }
    }
  }
}
</script>
<style>
</style>
