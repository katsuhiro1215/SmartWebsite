<script setup>
import { defineProps } from "vue";

const props = defineProps({
  textBlocks: {
    type: Array,
    required: true,
  },
  scrollTime: {
    type: Number,
    default: 20,
  },
});
</script>

<template>
  <div
    class="scroll relative flex overflow-hidden -rotate-3"
    :style="`--t: ${scrollTime}s`"
  >
    <div
      class="whitespace-nowrap"
      v-for="textBlock in textBlocks"
      :key="textBlock.id"
    >
      <span
        v-for="text in textBlock.texts"
        :key="text"
        class="inline-flex m-4 bg-slate-900 text-white py-3 px-4 rounded-md transition duration-75 hover:bg-green-300 leading-3 cursor-pointer"
      >
        {{ text }}
      </span>
    </div>
    <div
      class="whitespace-nowrap"
      v-for="textBlock in textBlocks"
      :key="textBlock.id"
    >
      <span
        v-for="text in textBlock.texts"
        :key="text"
        class="inline-flex m-4 bg-slate-900 text-white py-3 px-4 rounded-md transition duration-75 hover:bg-green-300 leading-3 cursor-pointer"
      >
        {{ text }}
      </span>
    </div>
  </div>
</template>

<style scoped>
.scroll {
  -webkit-mask-image: linear-gradient(
    90deg,
    transparent,
    #fff 20%,
    #fff 80%,
    transparent
  );
}
.scroll div {
  animation: animate var(--t) linear infinite;
  animation-delay: calc(var(--t) * -1);
}
.scroll div:nth-child(2) {
  animation: animate2 var(--t) linear infinite;
  animation-delay: calc(var(--t) / -2);
}
@keyframes animate {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(-100%);
  }
}
@keyframes animate2 {
  0% {
    transform: translateX(0%);
  }
  100% {
    transform: translateX(-200%);
  }
}
</style>
