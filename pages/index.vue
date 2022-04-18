<template>
  <div>
    
    <CallToAction />
    <colored-text :title="introductionTitle" :text="introductionText" />
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
  },
  data: () => {
    return {
      introductionTitle: `Willkommen bei Glasdesign Wolffhardt`,
      introductionText: `
        Der traditionsreiche Familienbetrieb im Zentrum von
        Tulln wird in vierter Generation von Andreas Wolffhardt
        geführt.
        Er setzt neben traditioneller Glaserei auf individuelle
        und künstlerisch gestaltete Glasprodukte und Spiegel
        und bringt seine Erfahrung als Glas-Sachverständiger ein.
        Die Zusammenarbeit mit anderen Handwerksbranchen, wie
        Tischler, Installateure oder Innenausstatter etc. wird
        forciert, um dem Kunden ein ganzheitliches Produkt bieten
        zu können.
      `,
    };
  }
});
</script>
