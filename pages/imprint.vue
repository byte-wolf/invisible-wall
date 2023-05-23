<template>
  <div class="pb-8">
      <card-heading :title="'Impressum'" :text="''" />

      <div class="bg-white rounded-md container mx-auto p-5">
        Wolffhardt G.m.b.H.

        <div class="font-bold mt-4">Glasermeister Andreas Wolffhardt</div>
        <div>Rudolfstraße 4</div>
        <div>3430 Tulln</div>
        <div>Österreich</div>

        <div class="mt-4">Tel.: 02272 / 627 80
        </div>
        <div>E-Mail: glas@tulln.net</div>
        <div>Website: www.glasdesign.at</div>

        <div class="font-bold mt-4">Firmenbuchnummer</div>
        <div>102682d</div>

        <div class="font-bold mt-4">Umsatzsteueridentifikationsnummer</div>
        <div>ATU20253204</div>

        <div class="font-bold mt-4">Firmengericht</div>
        <div>Landesgericht St. Pölten</div>

        <div class="font-bold mt-4">Behörde gem. ECG (E-Commerce Gesetz)</div>
        <div>Bezirkshauptmannschaft Tulln</div>
      </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import CardHeading from '~/components/CardHeading.vue'
export default Vue.extend({
  components: { CardHeading },
  head: () => {
    return {
      title: 'Impressum'
    };
  },
})
</script>

<style>

</style>