<script setup>
defineProps({ modelValue: String });
let emit = defineEmits(["update:modelValue"]);

function onTabPress(e) {
  let textarea = e.target;
  let val = textarea.value,
    start = textarea.selectionStart,
    end = textarea.selectionEnd;
  textarea.value = val.substr(0, start) + "\t" + val.substr(end);
  textarea.selectionStart = t.selectionEnd = start + 1;
}

function update() {
  emit("update:modelValue", e.target.value);
}
</script>

<template>
  <textarea
    @keydown.tab.prevent="onTabPress"
    @keyup="update"
    v-text="modelValue"
  />
</template>
