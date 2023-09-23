<template>
  <router-link :to="props.route" class="text-gray-400 font-bold">
    <div class="flex flex-col items-center">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="w-6 h-6"
      >
        <path stroke-linecap="round" stroke-linejoin="round" :d="props.icon" />
      </svg>
      <span>{{ props.label }}</span>
    </div>
  </router-link>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
  label: String,
  icon: String,
  route: String,
});
</script>
