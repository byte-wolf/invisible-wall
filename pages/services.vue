<template>
  <div>
      <services/>
      <colored-text/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import ColoredText from '~/components/ColoredText.vue'
import Services from '~/components/Services.vue'
export default Vue.extend({
  components: { Services, ColoredText },
    
})
</script>

<style>

</style>