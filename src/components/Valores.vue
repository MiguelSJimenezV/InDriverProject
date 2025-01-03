<script setup>
import SimpleCard from "./SimpleCard.vue";

let items = [
  {
    title: "Calidad",
    msg: "Nos esforzamos por ofrecer la más alta calidad en cada aspecto de nuestro servicio.",
  },
  {
    title: "Innovación",
    msg: "Buscamos constantemente nuevas formas de mejorar y adaptarnos a las necesidades de nuestros clientes.",
  },
  {
    title: "Compromiso",
    msg: "Estamos comprometidos con la satisfacción de nuestros clientes y el éxito de nuestros artistas asociados.",
  },
];
</script>
<template>
  <section class="bg-light py-5">
    <div class="container">
      <h2 class="text-center mb-4">Nuestros Valores</h2>
      <div class="row">
        <div class="col-md-4" v-for="item in items">
          <SimpleCard
            :title="item.title"
            :msg="item.msg"
            class="h-100"
          ></SimpleCard>
        </div>
      </div>
    </div>
  </section>
</template>
