<script setup>
import PrimaryButton from '@/Components/PrimaryButton.vue';
</script>

<template>
  <aside class="relative w-full flex flex-col justify-center items-center py-20 before:contents before:w-[1px] before:h-2 before:bg-slate-900 before:absolute before:top-0 before:left-1/2">
    <h3 class="text-4xl font-light mb-14 after:contents after:w-2 after:h-4 after:bg-slate-600">Contact</h3>
    <div class="text-center max-w-2xl leading-8">
      <p>10:00-19:00（平日）</p>
      <p>Tel03-1234-5678 / Fax03-1234-5678</p>
    </div>
    <div class="flex pt-14">
        <PrimaryButton>お問い合わせフォーム</PrimaryButton>
    </div>
  </aside>
</template>
