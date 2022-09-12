<script setup>
import { useTeamStore } from "@/stores/TeamStore";
let team = useTeamStore();
</script>
<template>
  <footer class="mt-12 bg-gray-100 py-4 text-center">
    <h5 class="font-semibold text-lg">{{ team.spotsRemaining }} Member Team</h5>
  </footer>
</template>
