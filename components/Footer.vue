<template>
    <footer class="shadow-md">
        <footer-links/>
        <hr class="border-gray-200 sm:mx-auto">
        <copyright-notice/>
    </footer>
</template>

<script lang="ts">
import Vue from 'vue'
import CopyrightNotice from './CopyrightNotice.vue';
import FooterLinks from './FooterLinks.vue';

export default Vue.extend({
    name: 'CompanyFooter',
    components: { CopyrightNotice, FooterLinks },
})
</script>