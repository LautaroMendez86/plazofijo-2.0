<script setup>
import NavItem from "@/components/navbar/NavItem.vue";
import { ref } from "vue";

const icons = ref({
  home: "M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25.",
  create: "M12 4.5v15m7.5-7.5h-15",
  profile:
    "M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z",
});
</script>

<template>
  <nav
    class="absolute bottom-0 w-screen rounded-t-2xl flex justify-around border-2 lg:border"
  >
    <nav-item route="/" :icon="icons.home" label="Home" />

    <nav-item route="/calculate" :icon="icons.create" label="Calcular" />

    <nav-item route="/profile" :icon="icons.profile" label="Perfil" />
  </nav>
</template>
