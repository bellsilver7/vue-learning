<script setup>
import { ref } from "vue";
import TabbaleTextarea from "@/components/TabbaleTextarea.vue";

let comment = ref("test value");

setTimeout(() => {
  comment.value = "It works!";
}, 2000);
</script>

<template>
  <main>
    <form action="">
      <TabbaleTextarea v-model="comment" style="width: 100%; height: 300px" />
    </form>
  </main>
</template>
