<script setup>
import { ref } from 'vue';

defineProps({
  placeholder: String,
  customClass: String,
});

const count = ref(0);
</script>

<template>
  <input :class="customClass" type="text" :placeholder="placeholder" />
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
