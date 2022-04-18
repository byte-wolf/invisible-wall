<template>
  <section class="bg-gray-100 py-8">
      <div class="container mx-auto flex justify-evenly flex-wrap">
          <div v-for="service in services" :key="service.title" class="max-w-sm w-96 bg-white shadow rounded-md overflow-hidden flex flex-col">
                
                <img class="w-full h-40 object-cover" :src="require('~/assets/img/'+ service.image)" alt="schiebetür" />
                
                <div class="px-6 py-4">

                    <div class="inline-flex items-center leading-none mb-4">
                        <div class="font-semibold text-xl flex-auto mr-2">
                            {{ service.title }}
                        </div>
                        <span v-if="service.tag != '' && service.tag" class="flex rounded-full px-2 py-1 bg-blue-200 text-blue-600 bg-opacity-100 uppercase font-semibold text-xs tracking-wide">
                            {{ service.tag }}
                        </span>
                    </div>

                    <p class="text-gray-700 text-base">
                        {{ service.description }}
                    </p>

                    

                </div>

                
                
                <a v-if="service.link" :href="service.link" class="mt-auto">
                    <div class="w-full bg-gray-100 text-gray-600 font-semibold px-6 py-3 uppercase text-xs text-center">
                        Mehr Informationen
                    </div>
                </a>
          </div>

          <!--<div class="max-w-sm w-52 bg-white shadow rounded-md overflow-hidden flex flex-col">
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
          </div>--> 
      </div>
  </section>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'ServicesList',
    data: () => {
        return {
            services: [
                

                {title: 'Glasdächer', description:
                    `Verandas, Carports und Vordächer schützen Sie oder Ihr Auto vor Niederschlag.`,
                    image: 'glass-dach.jpg', tag: ''},

                {title: 'Schiebetüren', description:
                    `Die Terrasse wird bei Bedarf mit beweglichen Glaselementen geschützt.
                    Wind und Wetter bleiben draussen. Der schöne Ausblick in die Natur
                    bleibt erhalten.`, image: 'glass-schiebetuere.jpg', tag: 'Beliebt'},

                {title: 'Bruchersatzgläser', description: `
                    Im Schadensfall reparieren wir professionell und kümmern uns um die Abwicklung mit ihrer Haushaltsversicherung. 
                `, image: 'glass-bruch.jpg'},
            ]
        };
    }
})
</script>

<style>

</style>