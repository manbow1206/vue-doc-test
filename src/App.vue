<template>
    <Lab>
      <template #header>
        <h1>Here might be a page title</h1>
      </template>
    
      <p>A paragraph for the main content.</p>
      <p>And another one.</p>
    
      <template #footer>
        <p>Here's some contact info</p>
      </template>
    </Lab>
</template>
<script>
import Lab from './components/Lab.vue'
export default {
  components: {
    Lab
  }
}
</script>
