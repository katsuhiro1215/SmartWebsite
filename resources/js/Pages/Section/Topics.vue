<script setup>
import PrimaryButton from '@/Components/PrimaryButton.vue';
import TopicsCard from "@/Components/Cards/TopicsCard.vue";
</script>

<template>
  <section class="w-full px-4 md:px-6 lg:px-14 py-20">
    <div class="w-full px-4 md:px-6 lg:px-14 py-6 mb-6">
      <h2 class="relative text-[240px] leading-none">
        T<span class="text-6xl absolute bottom-24 left-28">opics</span
        ><span class="text-2xl absolute bottom-12 left-30">更新情報</span>
      </h2>
    </div>
    <div class="w-full flex justify-around flex-wrap px-4 pb-20">
      <TopicsCard class="w-full top-0 mb-4 sm:w-2/5 sm:top-16 lg:w-1/5 lg:top-36" />
      <TopicsCard class="w-full top-0 mb-4 sm:w-2/5 sm:top-0 lg:w-1/5 lg:top-24" />
      <TopicsCard class="w-full top-0 mb-4 sm:w-2/5 sm:top-20 lg:w-1/5 lg:top-12" />
      <TopicsCard class="w-full top-0 mb-4 sm:w-2/5 sm:top-4 lg:w-1/5 lg:top-0" />
    </div>
    <div class="flex justify-end pt-14">
        <PrimaryButton>About</PrimaryButton>
    </div>
  </section>
</template>