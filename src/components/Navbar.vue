<template>
     <header class="flex justify-between items-center px-10 lg:px-24 py-12 text-white absolute top-0 left-0 w-full z-10">
        <h1 class="text-2xl font-bold">FurniShop</h1>
        <nav class="space-x-6 font-medium hidden lg:flex" >
            <a 
                href="#" 
                v-for="item in navbarList" 
                :key="item.name" 
                class="hover:text-gray-300 "
                :class="{'router-link-exact-active': item.link === '#'}"
            >{{ item.name }}</a>
        
        </nav>
        <button class="flex lg:hidden text-white">
            <img src="../assets/images/burger_menu.svg" alt="">
        </button>
  </header>  
</template>

<script setup>
import { ref } from 'vue';

const navbarList = ref([
    { name: 'Home', link: '#' },
    { name: 'About', link: '#' },
    { name: 'Features', link: '#' },
    { name: 'Contact', link: '#' }
])
</script>

<style lang="scss" scoped>

</style>