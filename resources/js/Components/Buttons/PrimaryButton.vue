<script setup>
import { computed } from "vue";
import { Link } from "@inertiajs/vue3";

const props = defineProps({
  buttonType: {
    type: String,
    default: "default",
  },
  buttonActionType: {
    type: String,
    default: "default",
  },
  href: {
    type: String,
    default: null,
  },
});

const buttonStyles = {
  default: {
    class: "bg-black text-white hover:bg-black/90",
  },
  primary: {
    class: "bg-blue-300 hover:bg-blue-300/90",
  },
  secondary: {
    class: "bg-slate-300 hover:bg-slate-300/90",
  },
  success: {
    class: "bg-green-300 hover:bg-green-300/90",
  },
  info: {
    class: "bg-sky-300 hover:bg-sky-300/90",
  },
  warning: {
    class: "bg-yellow-300 hover:bg-yellow-300/90",
  },
  danger: {
    class: "bg-red-300 hover:bg-red-300/90",
  },
  indigo: {
    class: "bg-indigo-300 hover:bg-indigo-300/90",
  },
};

const buttonClass = computed(() => buttonStyles[props.buttonActionType].class);
</script>

<template>
  <Link
    v-if="href"
    :href="href"
    class="inline-flex items-center justify-center whitespace-nowrap rounded-md text-sm font-medium transition-colors focus-visible:outline-none focus-visible:right-1 disabled:pointer-events-none disabled:opacity-50 shadow h-9 px-4 py-2"
    :class="buttonClass"
    :type="buttonActionType"
  >
    <slot></slot>
  </Link>

  <button
    v-else
    class="inline-flex items-center justify-center whitespace-nowrap rounded-md text-sm font-medium transition-colors focus-visible:outline-none focus-visible:right-1 disabled:pointer-events-none disabled:opacity-50 shadow h-9 px-4 py-2"
    :class="buttonClass"
    :type="buttonActionType"
  >
    <slot></slot>
  </button>
</template>