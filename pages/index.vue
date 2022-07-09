<script setup></script>

<template>
  <div class="bg-gray-200 px-20 py-32 flex place-content-center">
    <div
      class="bg-white rounded-lg h-full w-full py-10 px-16 justify-center items-center flex flex-col shadow-2xl"
    >
      <h1 class="text-3xl text-center font-semibold text-black">
        Sesión iniciada como ADMIN
      </h1>
      <div
        class="my-10 flex flex-col items-center shadow-xl border rounded-lg w-3/5 pb-20 pt-10 space-y-4"
      >
        <h1 class="text-2xl text-black">Acceso rápido</h1>
        <div class="space-x-4">
          <button class="btn btn-neutral text-white">Nuevo Cliente</button>
          <button class="btn btn-neutral text-white">Nuevo Pago</button>
        </div>
      </div>
    </div>
  </div>
</template>
