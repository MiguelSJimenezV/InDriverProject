<script setup>
defineProps({
  ids: {
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
  <div class="carousel-item h-100">
    <div class="container text-center w-100 h-100">
      <h1 class="display-4">{{ title }}</h1>
      <p class="lead mb-0">{{ msg }}</p>

  
        <a
          href="/upload#form"
  
          class="btn btn-warning m-3 text-dark text-decoration-none py-2 px-4"
          >{{ btn }}</a
        >

    </div>
  </div>
</template>
