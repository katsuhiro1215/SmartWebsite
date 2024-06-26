<script setup>
import { defineProps } from "vue";

const props = defineProps({
  imageBlocks: {
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
      class="flex items-center"
      v-for="imageBlock in imageBlocks"
      :key="imageBlock.id"
    >
      <img
        v-for="image in imageBlock.images"
        :key="image"
        :src="image"
        alt=""
        class="max-w-32 scale-75 filter grayscale-1 hover:grayscale-0 cursor-pointer"
      />
    </div>
    <div
      class="flex items-center"
      v-for="imageBlock in imageBlocks"
      :key="imageBlock.id"
    >
      <img
        v-for="image in imageBlock.images"
        :key="image"
        :src="image"
        alt=""
        class="max-w-32 scale-75 filter grayscale-1 hover:grayscale-0 cursor-pointer"
      />
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
