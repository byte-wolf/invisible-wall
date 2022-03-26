<template>
  <div>
    <Header/>
    <Jumbo />
    <CallToAction />
    <Services/>
    <Footer/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
  head: () => {
    return {
      title: 'Glasdesign Wolffhardt'
    };
  }
});
</script>
