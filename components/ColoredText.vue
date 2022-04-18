<template>
    <section>
        <div class="bg-blue-100 py-8">
            <div class="container mx-auto">
                <div class="text-blue-900  overflow-hidden rounded-lg p-6 h-auto">
                    <h2 class="text-xl font-bold mb-3">
                        {{ title }}
                    </h2>
                    
                    <p class="text-justify">
                        {{ text }}
                    </p>

                    <white-contact-button v-if="button"/>
                </div>
            </div>  
        </div>
    </section>
</template>

<script lang="ts">
import Vue from 'vue'
import WhiteContactButton from './WhiteContactButton.vue'
export default Vue.extend({
  components: { WhiteContactButton  },
    name: 'ColoredText',
    props: {
        title: String,
        text: String,
        button: Boolean,
    }
})
</script>

<style>

</style>