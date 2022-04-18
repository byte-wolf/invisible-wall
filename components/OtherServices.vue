<template>
    <section>
        <div class="container mx-auto flex-col mb-8 gap-10 items-start">
            <div class="bg-white rounded-lg overflow-hidden my-8">
                <div class="p-6">
                    <h1 class="font-bold text-xl mb-4">Andere Services</h1>
                    <p>
                        Hier finden Sie eine Liste mit häufig auftretenden Projekten die wir gerne übernehmen. 
                    </p>

                    <simple-list class="w-full mt-5"/>
                </div>
            </div>
            
        </div>
    </section>
</template>

<script lang="ts">
import Vue from 'vue'
import CardHeading from './CardHeading.vue'
export default Vue.extend({
  components: { CardHeading },
    name: 'OtherServices',
})
</script>

<style>

</style>