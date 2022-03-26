<template>
    <div class="py-4 px-6 sm:flex sm:items-center sm:justify-between container mx-auto">
        <a href="https://www.glasdesign.at" class="flex items-center mb-4 sm:mb-0">
            <logo/>
            <span class="self-center text-xl font-semibold whitespace-nowrap dark:text-white">
                Glaserei Wolffhardt
            </span>
        </a>
        <ul class="flex flex-wrap items-center text-sm text-gray-500 sm:mb-0 dark:text-gray-400">
            <li>
                <a href="#" class="mr-4 text-blue-800 md:mr-6 ">About</a>
            </li>
            <li>
                <a href="#" class="mr-4 text-blue-800 md:mr-6">Privacy Policy</a>
            </li>
            <li>
                <a href="#" class="mr-4 text-blue-800 md:mr-6 ">Licensing</a>
            </li>
            <li>
                <a href="#" class="text-blue-800">Contact</a>
            </li>
        </ul>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Logo from './Logo.vue'
export default Vue.extend({
    name: 'FooterLinks',
    components: { Logo },
})
</script>