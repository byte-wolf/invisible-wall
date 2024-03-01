<template>
    <div class="py-4 px-6 sm:flex sm:items-center sm:justify-between container mx-auto">
        <a href="https://www.glasdesign.at" class="flex items-center mb-4 sm:mb-0">
            <logo/>
            <span class="self-center text-xl font-semibold whitespace-nowrap dark:text-white">
                Glaserei Wolffhardt
            </span>
        </a>
        <ul class="flex flex-wrap items-center text-sm text-gray-500 sm:mb-0 dark:text-gray-400">
            <li v-for="item in linkItems" :key="item.title">
                <nuxt-link :to="'/' + item.page" class="footer-link-item">{{ item.title }}</nuxt-link>
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
    data: () => {
        return {
            linkItems: [
                {title: 'Impressum', page: 'imprint'},
                {title: 'Datenschutz', page: 'privacy'},
                //{title: 'Kontakt', page: 'contact'},
            ],
        };
    },
})
</script>