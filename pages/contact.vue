<template>
  <div>
      <contact-field/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import ContactField from '~/components/ContactField.vue'
export default Vue.extend({
    head: () => {
    return {
      title: 'Kontakt'
    };
  },
})
</script>

<style>

</style>
ContactField