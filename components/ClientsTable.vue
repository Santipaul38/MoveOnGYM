<script setup>
  defineProps({
    clients: {
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
                  #
                </th>
                <th
                  scope="col"
                  class="px-3 py-2 text-right text-lg font-semibold text-gray-900"
                >
                  Nombre
                </th>
                <th
                  scope="col"
                  class="px-3 py-2 text-left text-lg font-semibold text-gray-900"
                >
                  Apellido
                </th>
                <th
                  scope="col"
                  class="px-3 py-2 text-center text-lg font-semibold text-gray-900"
                >
                  DNI
                </th>
                <th
                  scope="col"
                  class="px-3 py-2 text-center text-lg font-semibold text-gray-900"
                >
                  Horario
                </th>
                <th
                  scope="col"
                  class="px-3 py-2 text-center text-lg font-semibold text-gray-900"
                >
                  Fecha de Inscripción
                </th>
              </tr>
            </thead>
            <tbody class="bg-white divide-y">
              <tr
                v-for="(client, index) in clients"
                :key="index"
                class="hover:bg-gray-100 cursor-pointer"
              >
                <td
                  class="whitespace-nowrap py-2 pl-4 pr-3 text-medium font-medium text-gray-900 sm:pl-6"
                >
                  {{ index }}
                </td>
                <td
                  class="whitespace-nowrap px-3 py-2 text-lg text-right text-black"
                >
                  {{ client.name }}
                </td>
                <td
                  class="whitespace-nowrap px-3 py-2 text-lg text-left text-black"
                >
                  {{ client.lastname }}
                </td>
                <td
                  class="whitespace-nowrap px-3 py-2 text-lg text-center text-black"
                >
                  {{ client.dni }}
                </td>
                <td
                  class="whitespace-nowrap px-3 py-2 text-lg text-center text-black"
                >
                  {{ client.schedule }}
                </td>
                <td
                  class="whitespace-nowrap px-3 py-2 text-lg text-center text-black"
                >
                  {{ client.inscription_date }}
                </td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>
