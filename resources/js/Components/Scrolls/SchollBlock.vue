<script setup>
import TextScrollBlock from "@/Components/Scrolls/TextScrollBlock.vue";
import ImageScrollBlock from "@/Components/Scrolls/ImageScrollBlock.vue";

const textBlocks1 = [
  {
    id: 1,
    texts: ["HTML", "CSS", "JavaScript", "NodeJS", "VueJS", "ReactJS"],
  },
];

const textBlocks2 = [
  {
    id: 2,
    texts: ["PHP", "Ruby", "Python", "Java", "Go", "Rust"],
  },
];

const imageBlocks1 = [
  {
    id: 1,
    images: [
      "images/kyoto.jpg",
      "images/kyoto.jpg",
      "images/kyoto.jpg",
      "images/kyoto.jpg",
      "images/kyoto.jpg",
      "images/kyoto.jpg",
    ],
  },
];

const imageBlocks2 = [
  {
    id: 2,
    images: [
      "images/kyoto.jpg",
      "images/kyoto.jpg",
      "images/kyoto.jpg",
      "images/kyoto.jpg",
      "images/kyoto.jpg",
      "images/kyoto.jpg",
    ],
  },
];
</script>

<template>
  <div class="flex flex-col justify-center w-[800px] mx-auto py-20">
    <TextScrollBlock :textBlocks="textBlocks1" scrollTime="20" />
    <ImageScrollBlock :imageBlocks="imageBlocks1" scrollTime="30" />
    <TextScrollBlock :textBlocks="textBlocks2" scrollTime="40" />
    <ImageScrollBlock :imageBlocks="imageBlocks2" scrollTime="25" />
  </div>
</template>

<style>
.scroll img {
  filter: grayscale(1);
}
.scroll img:hover {
  filter: grayscale(0);
}
</style>
