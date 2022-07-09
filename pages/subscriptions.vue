<script setup>
  const subscriptions = ref([
    {
      name: "Musculación hasta 2 dias personalizado",
      price: "2500",
      expiration_day: "12",
      expiration_add: "",
    },
    {
      name: "3 días o mas libre",
      price: "2500",
      expiration_day: "12",
      expiration_add: "",
    },
    {
      name: "2 días o menos libre",
      price: "2000",
      expiration_day: "12",
      expiration_add: "",
    },
    {
      name: "Musculación 3 o mas dias personalizado",
      price: "2800",
      expiration_day: "12",
      expiration_add: "",
    },
  ]);
</script>

<template>
  <div class="max-h-full w-full">
    <div class="bg-white mx-10 my-10 px-10 py-8 rounded-lg shadow-2xl">
      <div class="w-full flex justify-center border-b-2">
        <span class="text-black text-center font-semibold text-5xl mb-10"
          >Cuotas</span
        >
      </div>
      <SubscriptionsTable :subscriptions="subscriptions" />
    </div>
  </div>
</template>
