<template>
    <section>
        <div class="container mx-auto pb-8 flex flex-row flex-wrap justify-start items-start content-start md:gap-10">
            
            <contact-card />

            <div class="flex-grow overflow-hidden">
                <div class="mt-8 bg-white overflow-hidden shadow rounded-lg p-6 h-auto">
                    <h2 class="text-lg font-medium">
                        Glasereibetrieb
                    </h2>
                    <h1 class="text-xl font-bold mb-5">
                        Aktuelle Öffnungszeiten
                    </h1>
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
                    <nuxt-link to="/contact">
                        <contact-button />
                    </nuxt-link>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import ContactButton from './ContactButton.vue'
import ContactCard from './ContactCard.vue'
export default {
    name: 'CallToAction',
    components: {ContactButton, ContactCard},
    
}
</script>
        