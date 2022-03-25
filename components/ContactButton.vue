<template>
    <div class="text-left">
        <div class="p-2 bg-blue-100 items-center text-blue-900 leading-none rounded-full flex inline-flex" role="alert">
            <span class="flex rounded-full bg-blue-500 text-blue-100 uppercase px-2 py-1 text-xs font-bold mr-3">
                Individuell
            </span>
            <span class="font-semibold mr-2 text-left flex-auto">
                Kontaktieren Sie uns!
            </span>
            <svg class="fill-current opacity-75 h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M12.95 10.707l.707-.707L8 4.343 6.586 5.757 10.828 10l-4.242 4.243L8 15.657l4.95-4.95z"/></svg>
        </div>
    </div>
        
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'ContactButton',
})
</script>