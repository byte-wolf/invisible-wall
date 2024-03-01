<template>
    <!--<CallToAction />
    <colored-text :title="introductionTitle" :text="introductionText" />
    <Services     />-->

    <div>
      <div class="flex items-center justify-center py-6 h-full">
      <div class="rounded-lg p-[4px] bg-gradient-to-b from-cyan-50 to-blue-300 shadow-lg shadow-blue-400/30">
        <div class="rounded-lg  p-5 bg-white">
          <h1 class="text-lg font-semibold">Diese Website befindet sich im Wartungsmodus</h1>
          <p>Wir bitten um Ihr Verständnis.</p>

          <div class="flex justify-center py-8">
            <svg class="lucide lucide-construction size-32 text-gray-300" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="6" width="20" height="8" rx="1"/><path d="M17 14v7"/><path d="M7 14v7"/><path d="M17 3v3"/><path d="M7 3v3"/><path d="M10 14 2.3 6.3"/><path d="m14 6 7.7 7.7"/><path d="m8 6 8 8"/></svg>
          </div>
          <p>Bei Fragen wenden Sie sich bitte an <span>glas@tulln.net</span></p>
        </div>
      </div>
    </div>

    <div class="py-4"></div>
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
