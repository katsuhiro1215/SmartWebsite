<script setup>
import HeaderNavigation from '@/Layouts/HeaderNavigation.vue';
import ApplicationLogo from '@/Components/ApplicationLogo.vue';
import MenuBar from '@/Components/MenuBar.vue';
</script>

<template>
  <header class="fixed top-0 left-0 w-full h-16 border-b-2 z-10 bg-white/30">
    <div class="flex justify-between py-3 md:py-4 px-4 lg:px-14 mx-auto">
      <div class="flex items-center gap-2">
        <ApplicationLogo class="size-8" />
        <h1 class="text-xl font-semibold">Smart Sprouts</h1>
      </div>
      <div class="flex justify-end items-center gap-6">
        <HeaderNavigation />
        <MenuBar />
      </div>
    </div>
  </header>
</template>

