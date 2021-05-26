<template>
    <Lab>
      <template v-slot:default="slotProps">
        {{ slotProps.user.lastName }}
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
