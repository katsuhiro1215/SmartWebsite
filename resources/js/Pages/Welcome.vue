<script setup>
import { Head, Link } from "@inertiajs/vue3";
import Header from "@/Layouts/Header.vue";
import Footer from "@/Layouts/Footer.vue";
import Hero from "@/Pages/Section/Hero.vue";
import Topics from "@/Pages/Section/Topics.vue";
import About from "@/Pages/Section/About.vue";
import Service from "@/Pages/Section/Service.vue";
import Banner from "@/Pages/Section/Banner.vue";
import Contact from "@/Pages/Section/Contact.vue";
</script>

<template>
  <Head title="Welcome" />

  <div class="relative w-full h-full bg-slate-100">
    <Header />
    <main class="relative w-full min-h-screen pt-16">
      <Hero />
      <About />
      <Service />
      <Banner />
      <Topics />
    </main>
    <Contact />
    <Footer />
  </div>
</template>

<style>
.bg-dots-darker {
  background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(0,0,0,0.07)'/%3E%3C/svg%3E");
}
@media (prefers-color-scheme: dark) {
  .dark\:bg-dots-lighter {
    background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(255,255,255,0.07)'/%3E%3C/svg%3E");
  }
}
</style>
