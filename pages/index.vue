<template>
  <div>
    
    <CallToAction />
    <colored-text />
    <Services     />

  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import ColoredText from '~/components/ColoredText.vue';

export default Vue.extend({
  name: 'IndexPage',
  components: { ColoredText },
  head: () => {
    return {
      title: 'Glasdesign Wolffhardt'
    };
  }
});
</script>
