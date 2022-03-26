<template>
  <section>
      <div class="bg-gray-100 w-full">
        <div class="container mx-auto pb-8 flex flex-row flex-wrap justify-start items-start content-start md:gap-10">
            <div class="mt-8 bg-white overflow-hidden shadow rounded-lg p-6 sm:w-auto w-full pr-20">
                <h3 class="text-lg font-medium">
                    Glasermeister
                </h3>
                <h2 class="text-xl font-bold mb-5">
                    Andreas Wolffhardt
                </h2>
                <p>
                    Rudolfstraße 4
                    <br>
                    3430 Tulln
                    <br>
                    02272 / 627 80-0
                    <br>
                    glas@tulln.net
                    <br>
                    <a href="https://www.glasdesign.at" class="text-blue-800">www.glasdesign.at</a>
                </p>
            </div>
            <div class="flex-grow overflow-hidden">
                <div class="mt-8 bg-white overflow-hidden shadow rounded-lg p-6 h-auto">
                    <h3 class="text-lg font-medium">
                        Glasereibetrieb
                    </h3>
                    <h2 class="text-xl font-bold mb-5">
                        Aktuelle Öffnungszeiten
                    </h2>
                    <table class="text-left">
                        <tr>
                            <th class="pr-2 sm:pr-10 font-semibold align-top">Büro</th>
                            <td>Mo. - Do.</td>
                            <td>von 08:00 bis 12:00</td>
                        </tr>
                        <tr>
                            <td></td>
                            <td></td>
                            <td>von 13:00 bis 17:00</td>
                        </tr>
                        <tr>
                            <th></th>
                            <td>Fr.</td>
                            <td>von 08:00 bis 12:00</td>
                        </tr>
                        <tr>
                            <td class="py-3"></td>
                        </tr>
                        <tr>
                            <th class="pr-2 sm:pr-10 font-semibold align-top">Telefondienst</th>
                            <td>Mo. - Fr.</td>
                            <td>von 13:00 bis 17:00</td>
                        </tr>
                    </table>

                    <h3 class="font-semibold mt-6 mb-3">
                        Werkstätte und Montagen:
                    </h3>
                    <a href="/contact">
                        <contact-button />
                    </a>
                </div>
            </div>
        </div>

        <div class="bg-blue-100 py-8">
            <div class="container mx-auto">
                <div class="text-blue-900  overflow-hidden rounded-lg p-6 h-auto">
                    <h2 class="text-xl font-bold mb-3">
                        Willkommen bei Glasdesign Wolffhardt
                    </h2>
                    
                    <p class="text-justify">
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
                    </p>
                </div>
            </div>  
        </div>
    </div>
  </section>
</template>

<script>
import ContactButton from './ContactButton.vue'
export default {
    name: 'CallToAction',
    components: {ContactButton}
}
</script>
        