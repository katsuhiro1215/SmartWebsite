<script setup>
import { Link } from '@inertiajs/vue3';

</script>

<template>
  <nav>
    <ul class="flex items-center gap-4">
      <li>
        <Link href=""><span class="text-blue-500 font-semibold">S</span>tudy</Link>
      </li>
      <li>
        <Link href=""><span class="text-green-500 font-semibold">M</span>ark</Link>
      </li>
      <li>
        <Link href=""><span class="text-yellow-500 font-semibold">A</span>bout</Link>
      </li>
      <li>
        <Link href=""><span class="text-pink-500 font-semibold">R</span>eality</Link>
      </li>
      <li>
        <Link href=""><span class="text-indigo-500 font-semibold">T</span>opics</Link>
      </li>
    </ul>
  </nav>
</template>

