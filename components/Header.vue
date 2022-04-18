<template>
    <header>
        <nav class="bg-white sm:bg-opacity-95 border-gray-200 px-2 sm:px-4 py-3 rounded dark:bg-gray-800 shadow-sm">
            <div class="container flex flex-wrap justify-between items-center mx-auto px-6">
                <nuxt-link to="/" class="flex items-center">
                    <logo/>
                    <span class="self-center text-xl font-semibold whitespace-nowrap dark:text-white">wolffhardt</span>
                </nuxt-link>
                <button data-collapse-toggle="mobile-menu" type="button" class="inline-flex items-center p-2 ml-3 text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="mobile-menu" aria-expanded="false" @click="showMenu = !showMenu">
                    <span class="sr-only">Open main menu</span>
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
                    <svg class="hidden w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                </button>
                <div id="mobile-menu" :class="{hidden: !showMenu}" class=" w-full md:block md:w-auto">
                <ul class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium">
                    <li @click="showMenu = false" v-for="item in menuItems" :key="item.title">
                        <nuxt-link :to="'/'+item.page" :class="{'link-item-active': $nuxt.$route.path.replace('/', '') === item.page}" class="link-item">
                            {{item.title}}
                        </nuxt-link>
                    </li>
                </ul>
                </div>
            </div>
        </nav>
    </header>
</template>

<script lang="ts">
import Vue from 'vue'
import Logo from './Logo.vue';

export default Vue.extend({
  name: 'MainHeader',
  components: { Logo },
  data: () => {
      return {
          showMenu: false,
          menuItems: [
              {title: 'Home', page: ''},
              {title: 'Leistungen', page: 'services'},
              {title: 'Galerie', page: 'gallery'},
              {title: 'Kontakt', page: 'contact'},
          ],
      };
  }
})
</script>