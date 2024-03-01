<template>
    <div class="text-center text-xs p-6 bg-gray-50">
        <span>© {{year}} Copyright:</span>
        <a class="text-blue-800" href="https://www.glasdesign.at">
            Andreas Wolffhardt
        </a>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'CopyrightNotice',
    data: () => {
        return {
            year: new Date().getFullYear(),
        };
    }
})
</script>