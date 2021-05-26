<template>
    <Lab v-slot="slotProps">
        {{ slotProps.user.lastName }}
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
