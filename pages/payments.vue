<script setup>
  const payments = ref([
    {
      amount: "2400",
      subscription: "Musculación 3 o mas días personalizado",
      client: "Santiago Paul",
      month: "Febrero",
      payment_date: "02/07/2022 - 16:00",
    },
    {
      amount: "2400",
      subscription: "Musculación 3 o mas días personalizado",
      client: "Santiago Paul",
      month: "Febrero",
      payment_date: "02/07/2022 - 16:00",
    },
    {
      amount: "2400",
      subscription: "Musculación 3 o mas días personalizado",
      client: "Santiago Paul",
      month: "Febrero",
      payment_date: "02/07/2022 - 16:00",
    },
    {
      amount: "2400",
      subscription: "Musculación 3 o mas días personalizado",
      client: "Santiago Paul",
      month: "Febrero",
      payment_date: "02/07/2022 - 16:00",
    },
    {
      amount: "2400",
      subscription: "Musculación 3 o mas días personalizado",
      client: "Santiago Paul",
      month: "Febrero",
      payment_date: "02/07/2022 - 16:00",
    },
  ]);
</script>

<template>
  <div class="max-h-full w-full">
    <div class="bg-white mx-10 my-10 px-10 py-8 rounded-lg shadow-2xl">
      <div class="w-full flex justify-center border-b-2">
        <span class="text-black text-center font-semibold text-5xl mb-10"
          >Pagos</span
        >
      </div>
      <PaymentsTable :payments="payments" />
    </div>
  </div>
</template>
