<script setup>
defineProps({
  title: {
    type: String,
    required: true,
  },
  msg: {
    type: String,
    required: true,
  },
});
</script>
<template>
  <div>
    <h2 class="mb-4">{{ title }}</h2>
    <p class="w-50">
      {{ msg }}
    </p>
  </div>
</template>
