<script setup>
  import { ref } from "@vue/reactivity";

  const clients = ref([
    {
      name: "Santiago",
      lastname: "Paul",
      dni: "42487270",
      schedule: "06:00",
      inscription_date: "21/05/2022 - 14:20",
    },
    {
      name: "Emiliano 'La nutria'",
      lastname: "Paul",
      dni: "50264568",
      schedule: "06:00",
      inscription_date: "21/05/2022 - 14:20",
    },
    {
      name: "Santiago",
      lastname: "Paul",
      dni: "42487270",
      schedule: "06:00",
      inscription_date: "21/05/2022 - 14:20",
    },
    {
      name: "Santiago",
      lastname: "Paul",
      dni: "42487270",
      schedule: "06:00",
      inscription_date: "21/05/2022 - 14:20",
    },
    {
      name: "Santiago",
      lastname: "Paul",
      dni: "42487270",
      schedule: "06:00",
      inscription_date: "21/05/2022 - 14:20",
    },
    {
      name: "Santiago",
      lastname: "Paul",
      dni: "42487270",
      schedule: "06:00",
      inscription_date: "21/05/2022 - 14:20",
    },
    {
      name: "Santiago",
      lastname: "Paul",
      dni: "42487270",
      schedule: "06:00",
      inscription_date: "21/05/2022 - 14:20",
    },
    {
      name: "Santiago",
      lastname: "Paul",
      dni: "42487270",
      schedule: "06:00",
      inscription_date: "21/05/2022 - 14:20",
    },
  ]);
</script>

<template>
  <div class="max-h-full w-full">
    <div class="bg-white mx-10 my-10 px-10 py-8 rounded-lg shadow-2xl">
      <div class="w-full flex justify-center border-b-2">
        <span class="text-black text-center font-semibold text-5xl mb-10"
          >Clientes</span
        >
      </div>
      <ClientsTable :clients="clients" />
    </div>
  </div>
</template>
