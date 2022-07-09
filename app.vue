<script setup>
  const route = useRoute();
</script>

<template>
  <div class="min-h-screen flex flex-col justify-between bg-gray-200">
    <Navbar class="z-10" />
    <NuxtPage class="h-full z-0" />
    <Footer class="z-10" />
  </div>
</template>
