<template>
<section class="py-8">
    <div class="container mx-auto">
        <div class="bg-white rounded-md overflow-hidden">
            <div class="p-6">
                <h1 class="font-bold text-xl mb-4">Unsere Leistungen</h1>
                <p>
                    Wir bieten eine Vielzahl an verschiedenen Dienstleistungen an. Hier finden Sie eine Auswahl davon.
                </p>
            </div>
        </div>
    </div>
</section>
  
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'CardHeading',
    props: {
        title: String,
        text: String,
    }

})
</script>

<style>

</style>