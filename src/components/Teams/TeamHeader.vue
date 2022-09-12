<script setup>
import { useTeamStore } from "@/stores/TeamStore";
import AddMemebrModal from "@/components/Teams/AddMemberModal.vue";

let team = useTeamStore();
</script>
<template>
  <header class="flex justify-between px-6 py-4">
    <div>
      <AddMemebrModal />
    </div>
    <div>
      <h3 class="inline-flex items-center text-3xl relative">
        <img src="/smiley.png" alt="" class="mr-2" style="width: 40px" />
        {{ team.name }} Team
        <div
          class="bg-green-400 w-5 h-5 text-xs text-white rounded-full flex justify-center items-center absolute -right-4 -top-2"
        >
          {{ team.spots }}
        </div>
      </h3>
    </div>
  </header>
</template>
