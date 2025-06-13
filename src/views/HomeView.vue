<script setup>
import Navbar from '@/components/Navbar.vue';
import HeroSection from '@/components/HeroSection.vue';
import StateSection from '@/components/StateSection.vue';
</script>

<template>
    <section style="background-image: url('../src/assets/images/bg.jpg');" class="bg-right lg:bg-bottom 2xl:bg-bottom bg-cover bg-no-repeat h-screen px-10 md:px-24">
        <Navbar />
        <HeroSection />
    </section>
    <StateSection />
  
</template>
