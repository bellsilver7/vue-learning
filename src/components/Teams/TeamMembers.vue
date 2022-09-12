<script setup>
import TeamMember from "@/components/Teams/TeamMember.vue";
defineProps({ team: Object });
</script>
<template>
  <table class="table-fixed border-spacing-2 border-separate">
    <thead>
      <tr>
        <td class="text-left px-6 py-2">Name</td>
        <td class="text-left px-6 py-2">Email</td>
        <td class="text-left px-6 py-2">Status</td>
      </tr>
    </thead>
    <tbody>
      <TeamMember
        v-for="member in team.members"
        :key="member.id"
        :name="member.name"
        :email="member.email"
        :status="member.status"
      />
    </tbody>
  </table>
  <p
    class="text-right text-gray-600 italic"
    v-show="team.members.length === team.spots"
  >
    There are remaining team spots. Upgrade to add more.
  </p>
</template>
