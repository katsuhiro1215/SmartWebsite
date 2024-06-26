<script setup>
import ApplicationLogo from '@/Components/ApplicationLogo.vue';
import PrimaryButton from '@/Components/PrimaryButton.vue';
</script>

<template>
  <section class="relative w-full flex flex-col justify-center items-center py-20">
    <div class="absolute flex justify-center items-center">
      <ApplicationLogo class="w-80 h-80 opacity-20 z-0" />
    </div>
    <h3 class="text-4xl font-light mb-14 after:contents after:w-2 after:h-4 after:bg-slate-600">About</h3>
    <div class="text-center max-w-2xl leading-8">
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Natus quidem quaerat reiciendis amet quisquam veritatis aliquam, mollitia neque iste error!</p>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Natus quidem quaerat reiciendis amet quisquam veritatis aliquam, mollitia neque iste error!</p>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Natus quidem quaerat reiciendis amet quisquam veritatis aliquam, mollitia neque iste error!</p>
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Natus quidem quaerat reiciendis amet quisquam veritatis aliquam, mollitia neque iste error!</p>
    </div>
    <div class="flex pt-14">
        <PrimaryButton>About</PrimaryButton>
    </div>
  </section>
</template>