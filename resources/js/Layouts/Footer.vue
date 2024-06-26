<script setup>
import { ref } from "vue";
import { Link } from "@inertiajs/vue3";

const currentYear = ref(new Date().getFullYear());
</script>

<template>
  <footer class="w-full h-12 flex justify-center items-center bg-green-200">
    {{ currentYear }} &copy; Smart Sprouts theme by
    <Link href="https://katsucode.jp/">Katsucode</Link>
  </footer>
</template>
