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
  <div class="card p-4">
    <h4>{{ title }}</h4>
    <p>
      {{ msg }}
    </p>
  </div>
</template>
