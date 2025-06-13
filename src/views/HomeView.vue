<script setup>
import Navbar from '@/components/Navbar.vue';
import HeroSection from '@/components/HeroSection.vue';
</script>

<template>
    <section style="background-image: url('../src/assets/images/bg.jpg');" class="bg-right bg-cover">
      <div class="px-10 md:px-24">
        <Navbar />
        <HeroSection />
      </div>
    </section>
  
</template>
