<script setup>
  const route = useRoute();

  const routes = [
    { name: "Clientes", path: "/clients" },
    { name: "Pagos", path: "/payments" },
    { name: "Cuotas", path: "/subscriptions" },
  ];
</script>
<template>
  <div
    class="navbar lg:px-20 py-6 bg-neutral w-screen shadow-lg shadow-green-500"
  >
    <div class="navbar-start">
      <nuxt-link to="/">
        <img
          src="OnIcon.svg"
          class="h-10 hover:scale-110 cursor-pointer"
          alt="moveOn"
        />
      </nuxt-link>
    </div>
    <div class="navbar-center space-x-2">
      <nuxt-link
        v-for="r in routes"
        :key="r.path"
        :to="r.path"
        :class="
          route.path == r.path
            ? 'bg-black/20 btn font-medium'
            : 'btn font-light'
        "
        class="text-lg text-white"
        >{{ r.name }}</nuxt-link
      >
    </div>
    <div class="navbar-end space-x-2">
      <UserMenu />
    </div>
  </div>
</template>
