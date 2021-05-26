<template>
  <div class="home">
    <Lab>
      <template v-slot>Child Components</template>
    </Lab>
    <Lab>
      <template v-slot:add>渋谷</template>
    </Lab>
  </div>
</template>
<script>
import Lab from './components/Lab.vue'
export default {
  components: {
    Lab
  }
}
</script>
