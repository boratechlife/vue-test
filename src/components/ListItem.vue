<script setup>
import { ref } from 'vue';

defineProps({
  src: String,
  name: String,
  date: String,
});

const count = ref(0);
</script>

<template>
  <div class="flex gap-2 items-center w-full justify-between py-2">
    <div class="flex items-center gap-3">
      <div class="h-[20px] w-[20px] flex-none rounded-[2px] overflow-hidden">
        <img :src="src" class="flex h-[20px] w-[20px] object-cover" alt="" />
      </div>

      <div class="h-4 w-4 rounded-full bg-[#518103]"></div>
      <h4 class="text-sm font-medium">
        {{ name }}
      </h4>
    </div>
    <div class="flex items-center gap-2">
      <span class="text-sm">{{ date }}</span>
      <span>
        <svg
          width="16"
          height="16"
          viewBox="0 0 16 16"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M12.4714 5.47133C12.3463 5.34635 12.1768 5.27614 12 5.27614C11.8233 5.27614 11.6537 5.34635 11.5287 5.47133L8.47136 8.52866C8.34461 8.65032 8.17572 8.71826 8.00003 8.71826C7.82434 8.71826 7.65545 8.65032 7.52869 8.52866L4.47136 5.47133C4.34563 5.34989 4.17722 5.28269 4.00243 5.28421C3.82763 5.28573 3.66042 5.35584 3.53682 5.47945C3.41321 5.60306 3.3431 5.77026 3.34158 5.94506C3.34006 6.11986 3.40726 6.28826 3.52869 6.414L6.58536 9.47133C6.77108 9.65708 6.99158 9.80443 7.23425 9.90496C7.47692 10.0055 7.73702 10.0572 7.99969 10.0572C8.26237 10.0572 8.52247 10.0055 8.76514 9.90496C9.00781 9.80443 9.22831 9.65708 9.41403 9.47133L12.4714 6.414C12.5963 6.28898 12.6666 6.11944 12.6666 5.94266C12.6666 5.76589 12.5963 5.59635 12.4714 5.47133Z"
            fill="#626466"
          />
        </svg>
      </span>
    </div>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
