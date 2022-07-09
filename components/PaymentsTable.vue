<script setup>
  defineProps({
    payments: {
      type: Object,
      default: () => {},
    },
  });
</script>

<template>
  <div class="mt-8 max-h-full flex flex-col">
    <div
      class="-my-2 -mx-4 overflow-x-auto overflow-y-hidden sm:-mx-6 lg:-mx-8"
    >
      <div class="inline-block min-w-full py-2 align-middle md:px-6 lg:px-8">
        <div
          class="overflow-hidden shadow ring-1 ring-black ring-opacity-5 md:rounded-lg"
        >
          <table
            class="min-w-full divide-y divide-gray-300 max-h-full shadow-md"
          >
            <thead class="bg-gray-100">
              <tr>
                <th
                  scope="col"
                  class="py-2 pl-4 pr-3 text-left text-lg font-semibold text-gray-900 sm:pl-6"
                >
                  Monto
                </th>
                <th
                  scope="col"
                  class="px-3 py-2 text-center text-lg font-semibold text-gray-900"
                >
                  Suscripción
                </th>
                <th
                  scope="col"
                  class="px-3 py-2 text-center text-lg font-semibold text-gray-900"
                >
                  Cliente
                </th>
                <th
                  scope="col"
                  class="px-3 py-2 text-center text-lg font-semibold text-gray-900"
                >
                  Mes Pagado
                </th>
                <th
                  scope="col"
                  class="px-3 py-2 text-center text-lg font-semibold text-gray-900"
                >
                  Fecha de Recibo
                </th>
              </tr>
            </thead>
            <tbody class="bg-white divide-y">
              <tr
                v-for="payment in payments"
                :key="payment.client"
                class="hover:bg-gray-100 cursor-pointer"
              >
                <td
                  class="whitespace-nowrap py-2 pl-4 pr-3 text-medium text-gray-900 sm:pl-6"
                >
                  ${{ payment.amount }}
                </td>
                <td
                  class="whitespace-nowrap px-3 py-2 text-lg text-center text-black"
                >
                  {{ payment.subscription }}
                </td>
                <td
                  class="whitespace-nowrap px-3 py-2 text-lg text-center text-black"
                >
                  {{ payment.client }}
                </td>
                <td
                  class="whitespace-nowrap px-3 py-2 text-lg text-center text-black"
                >
                  {{ payment.month }}
                </td>
                <td
                  class="whitespace-nowrap px-3 py-2 text-lg text-center text-black"
                >
                  {{ payment.payment_date }}
                </td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>
