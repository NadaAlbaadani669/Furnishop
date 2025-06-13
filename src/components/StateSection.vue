<template>
    <section class="px-10 md:px-24 bg-transparent -mt-20">
    <div class="bg-teal-800 text-white py-12 px-4 rounded-2xl">
        <div class="max-w-6xl mx-auto w-full grid grid-cols-2 gap-y-2 lg:gap-y-0 lg:grid-cols-4 text-center divide-x divide-white/20">
            <div v-for="state in stats" :key="state" class="py-4 px-2">
                <h2 class="text-3xl font-bold mb-2">{{state.value}}</h2>
                <p class="text-sm uppercase tracking-wide">{{ state.label }}</p>
            </div>
            
        </div>
    </div>
    </section>

</template>

<script setup>
import { ref } from 'vue';

const stats = ref([
  { value: "7", label: "Year Experience" },
  { value: "2", label: "Opened in the country" },
  { value: "10k+", label: "Furniture Sold" },
  { value: "260+", label: "Variant Furniture" },
]);

</script>

<style lang="scss" scoped>

</style>