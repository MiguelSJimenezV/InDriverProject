<script setup>
defineProps({
  img: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  msg: {
    type: String,
    required: true,
  },
  btn: {
    type: String,
    required: true,
  },
});
</script>
<template>
    <div class="card-img-overlay">
      <h5 class="card-title">{{ title }}</h5>
      <p class="card-text">
        {{ msg }}
      </p>
      <a href="/about" class="btn btn-warning">{{ btn }}</a>
    </div>
</template>
