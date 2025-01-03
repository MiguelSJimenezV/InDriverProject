<script setup>
defineProps({
  title: {
    type: String,
    required: true,
  },
  msg1: {
    type: String,
    required: true,
  },
  msg2: {
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
  <section class="text-light">
    <h1 class="text-bassline py-1">{{ title }}</h1>
    <div class="row py-2">
      <div class="col-md-6 p-4">
        <p>{{ msg1 }}</p>
        <p>{{ msg2 }}</p>
        <button class="btn">
          <a href="#equipo" class="btn btn-warning h-100">{{ btn }}</a>
        </button>
      </div>
      <div class="col-md-6">
        <img
          src="../assets/img/ser-1.png"
          alt="Imagen de la empresa"
          class="img-fluid"
        />
      </div>
    </div>
  </section>
</template>
