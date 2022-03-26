<template>
  <section class="bg-gray-100 py-8">
      <div class="container mx-auto flex justify-center gap-10">
          <div class="max-w-sm w-52 bg-white shadow rounded-md overflow-hidden flex flex-col">
                <img class="w-full" src="@/assets/img/glass-schiebetür.jpg" alt="schiebetür">
                <div class="px-6 py-4">
                    
                    <span class="inline-block rounded-full px-2 py-1 bg-blue-200 text-blue-600 bg-opacity-100 uppercase font-semibold text-xs tracking-wide">
                        Beliebt
                    </span>

                    <div class="font-semibold mb-3">
                        Schiebetüren
                    </div>

                    

                    <p class="text-gray-700 text-base">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                        Voluptatibus quia, Nonea!
                    </p>

                    
                </div>
                
                <a href="#" class="mt-auto">
                    <div class="w-full bg-gray-100 text-gray-600 font-semibold px-6 py-3 uppercase text-xs text-center">
                        Mehr Informationen
                    </div>
                </a>
          </div>

          <div class="max-w-sm w-52 bg-white shadow rounded-md overflow-hidden flex flex-col">
                <img class="w-full" src="@/assets/img/glass-türe.jpg" alt="schiebetür">
                <div class="px-6 py-4">
                    <div class="font-semibold mb-2">
                        Glastüren
                    </div>
                    <p class="text-gray-700 text-base">
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                        Voluptatibus quia, Nonea!
                    </p>
                </div>

                <a href="#" class="mt-auto">
                    <div class="w-full bg-gray-100 text-gray-600 font-semibold px-6 py-3 uppercase text-xs text-center">
                        Mehr Informationen
                    </div>
                </a>
          </div>
      </div>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'ServicesList',
})
</script>

<style>

</style>