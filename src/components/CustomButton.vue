<script setup>
import { ref } from 'vue';

defineProps({
  customClass: String,
});

const count = ref(0);
</script>

<template>
  <button :class="customClass">
    <slot></slot>
  </button>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
