<script setup>
import PrimaryButton from '@/Components/PrimaryButton.vue';
import Drop from "@/Components/Drop.vue";
</script>

<template>
  <section class="relative w-full h-[720px] flex items-center gap-6 px-14 py-20">
    <div class="relative w-1/2 h-3/5 top-1/4 left-40 order-2 md:order-none">
      <Drop />
    </div>
    <div class="w-1/2 top-1/4 px-4 md:px-6 lg:px-14 py-6 mb-6 order-1 md:order-none">
      <h2 class="relative text-[160px] leading-none">
        S<span class="text-4xl absolute bottom-16 left-24">ervices</span
        ><span class="text-lg absolute bottom-8 left-26">更新情報</span>
      </h2>
      <div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat, exercitationem nam minus placeat blanditiis voluptas libero delectus sed unde quasi.</p>
      </div>
      <div class="flex justify-end pt-14">
        <PrimaryButton>Service</PrimaryButton>
    </div>
    </div>
  </section>
</template>