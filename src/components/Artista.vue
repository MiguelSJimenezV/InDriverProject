<script setup>
defineProps({
  nombre: {
    type: String,
    required: true,
  },
  edad: {
    type: String,
    required: true,
  },
  descripcion: {
    type: String,
    required: true,
  },
  img: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  artista: {
    type: String,
    required: true,
  },
  genero: {
    type: String,
    required: true,
  },
  anio: {
    type: String,
    required: true,
  },
});
</script>
<template>
  <div class="card h-100">
    <div class="card-body">
      <h5 class="card-title">{{ nombre }}{{ title }}</h5>
      <p class="card-text">{{ edad }}{{ artista }}</p>
      <p class="card-text">{{ descripcion }}{{ anio }}</p>
      <p class="card-text">{{ genero }}</p>
      <p class="card-text">{{ tipo }}</p>
    </div>
  </div>
</template>
