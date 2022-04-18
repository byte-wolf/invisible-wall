<template>
  <div>
      <card-heading/>
      <services/>
      <other-services/>
      <colored-text :title="introductionTitle" :text="introductionText" :button="true"/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import CardHeading from '~/components/CardHeading.vue'
import ColoredText from '~/components/ColoredText.vue'
import OtherServices from '~/components/OtherServices.vue'
import Services from '~/components/Services.vue'
export default Vue.extend({
  components: { Services, ColoredText, CardHeading, OtherServices },
  data: () => {
    return {
      introductionTitle: `Sie haben einen anderen Wunsch? Kein Problem!`,
      introductionText: `
        Auch individuelle Projekte erledigen wir für Sie. Rufen Sie an,
        schreiben Sie eine E-Mail oder kommen Sie persönlich vorbei und
        lassen Sie sich beraten.
      `,
    };
  }
})
</script>

<style>

</style>