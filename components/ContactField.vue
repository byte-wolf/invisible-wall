<template>
  <section>
        <div class="container mx-auto pb-8 flex flex-row flex-wrap justify-start items-start content-start md:gap-10">
            
            <contact-card />

            <div class="flex-grow overflow-hidden">
                <div class="mt-8 bg-white overflow-hidden shadow rounded-lg p-6 h-auto">
                    <h1 class="text-lg font-medium">
                        Glasereibetrieb
                    </h1>
                    <h2 class="text-xl font-bold mb-3">
                        Kontakt und Anfragen
                    </h2>
                    
                    <div id="map-wrap" class="h-72 rounded-lg overflow-hidden">
                        <client-only>
                            <l-map 
                                :zoom=20
                                :center="[48.33174,16.05357]"
                                :options="{attributionControl: true}">

                                <l-tile-layer 
                                    url="https://{s}.tile.osm.org/{z}/{x}/{y}.png" 
                                    :attribution="attribution">
                                
                                </l-tile-layer>
                                <l-marker :lat-lng="[48.33174,16.05357]">
                                    <l-tooltip :options="{permanent: true}">
                                        Rudolfstraße 4
                                    </l-tooltip>
                                </l-marker>

                                <l-marker :lat-lng="[48.33185, 16.05453]">
                                    <l-tooltip :options="{permanent: true}">
                                        Nibelungengasse 3
                                    </l-tooltip>
                                </l-marker>
                            </l-map>
                        </client-only>
                    </div>

                    <div class="mt-5 bg-blue-50 p-2 text-blue-900 font-semibold text-sm rounded-lg border-2 border-l-4 border-blue-100 flex items-center gap-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zm-7-4a1 1 0 11-2 0 1 1 0 012 0zM9 9a1 1 0 000 2v3a1 1 0 001 1h1a1 1 0 100-2v-3a1 1 0 00-1-1H9z" clip-rule="evenodd" />
                        </svg>
                        <span>
                            Beachten Sie bitte stets unsere Öffnungszeiten.
                        </span>
                    </div>

                    <hr class="my-5 border-none">

                    <h2 class="font-medium text-lg">
                        Sie möchten uns persönlich kontaktieren?
                    </h2>

                    <div>
                        Standort: Rudolfstraße 4
                    </div>
                    <div>
                        Zufahrt: Nibelungengasse 3
                    </div>

                    <hr class="my-5">

                    <h2 class="font-medium text-lg">
                        Sie haben natürlich auch die Möglichkeit uns per E-Mail oder Telefon zu erreichen.
                    </h2>
                    
                    

                    <div class="mt-4 rounded-full bg-blue-100 inline-flex items-center leading-none">
                        <div class="p-2 rounded-full bg-blue-500 inline-flex text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                                <path d="M2 3a1 1 0 011-1h2.153a1 1 0 01.986.836l.74 4.435a1 1 0 01-.54 1.06l-1.548.773a11.037 11.037 0 006.105 6.105l.774-1.548a1 1 0 011.059-.54l4.435.74a1 1 0 01.836.986V17a1 1 0 01-1 1h-2C7.82 18 2 12.18 2 5V3z" />
                            </svg>
                        </div>
                        <span class="font-semibold mr-2 text-left flex-auto text-blue-900 px-3">
                            02272 / 627 80-0
                        </span>
                    </div>

                    <div class="mt-4 rounded-full bg-blue-100 inline-flex items-center leading-none">
                        <div class="p-2 rounded-full bg-blue-500 inline-flex text-white">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                                <path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z" />
                                <path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z" />
                            </svg>
                        </div>
                        <span class="font-semibold mr-2 text-left flex-auto text-blue-900 px-3">
                            glas@tulln.net
                        </span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script lang="ts">
import Vue from 'vue';
export default Vue.extend({
    name: 'ContactField',
    data: () => {
        return {
            attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors',
        };
    }
})
</script>

<style>

</style>