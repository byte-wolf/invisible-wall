<template>
  <div class="bg-white rounded-lg overflow-hidden border border-gray-200 w-96">
      <div v-for="element in listElements" :key="element" class="border-b border-gray-200 px-4 py-2">
          {{ element }}
      </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'SimpleList',
    data: () => {
        return {
            listElements: [
                'Ganzglastüren',
                'Glasdächer',
                'Hustenschutzglas u. Trennwände',
                'Schrankschiebetüren',
                'Glasduschen',
                'Dekorative Glasanwendung',
                'Sicherheitsglas',
                'Spiegel u. Wandbeläge aus Glas',
                'Schalterboxen transparent',
                'Reparaturen & Austauschglas',
                'Glashandel',
            ]
        };
    }
})
</script>

<style>

</style>