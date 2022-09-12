<script setup></script>

<template>
  <header class="flex justify-between px-6 py-4">
    <div>
      <button
        class="bg-green-500 hover:bg-green-600 text-white px-4 py-2 rounded disabled:bg-gray-400"
        :disabled="true"
      >
        Add Member (0 Spots Left)
      </button>
    </div>
    <div>
      <h3 class="inline-flex items-center text-3xl relative">
        <img src="/smiley.png" alt="" class="mr-2" style="width: 40px" />
        Smiley Team
        <div
          class="bg-green-400 w-5 h-5 text-xs text-white rounded-full flex justify-center items-center absolute -right-4 -top-2"
        >
          5
        </div>
      </h3>
    </div>
  </header>

  <div class="flex flex-col gap-y-3">
    <table class="table-fixed border-spacing-2 border-separate">
      <thead>
        <tr>
          <td class="text-left px-6 py-2">Name</td>
          <td class="text-left px-6 py-2">Email</td>
          <td class="text-left px-6 py-2">Status</td>
        </tr>
      </thead>
      <tbody>
        <tr class="bg-gray-100 px-12">
          <td class="text-xl font-medium flex items-center gap-x-4 px-6 py-4">
            <img
              src="https://i.pravatar.cc/50?u=steve@doe.com"
              alt=""
              class="rounded-xl"
            />
            Steven Doe
          </td>
          <td class="text-gray-500 px-6 py-4">steven@doe.com</td>
          <td class="px-6 py-4">
            <button class="text-green-400 text-xl">Active</button>
          </td>
        </tr>
        <tr class="bg-gray-100 px-12">
          <td class="text-xl font-medium flex items-center gap-x-4 px-6 py-4">
            <img
              src="https://i.pravatar.cc/50?u=steve@doe.com"
              alt=""
              class="rounded-xl"
            />
            Steven Doe
          </td>
          <td class="text-gray-500 px-6 py-4">steven@doe.com</td>
          <td class="px-6 py-4">
            <button class="text-green-400 text-xl">Active</button>
          </td>
        </tr>
        <tr class="bg-gray-100 px-12">
          <td class="text-xl font-medium flex items-center gap-x-4 px-6 py-4">
            <img
              src="https://i.pravatar.cc/50?u=steve@doe.com"
              alt=""
              class="rounded-xl"
            />
            Steven Doe
          </td>
          <td class="text-gray-500 px-6 py-4">steven@doe.com</td>
          <td class="px-6 py-4">
            <button class="text-green-400 text-xl">Active</button>
          </td>
        </tr>
      </tbody>
    </table>
    <p class="text-right text-gray-600 italic">
      There are remaining team spots. Upgrade to add more.
    </p>
  </div>
  <footer class="mt-12 bg-gray-100 py-4 text-center">
    <h5 class="font-semibold text-lg">Member Team</h5>
  </footer>
</template>
