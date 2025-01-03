<script setup>
import Artista from "./Artista.vue";
</script>
<template>
  <section class="py-3">
    <div class="container">
      <h2 class="text-center mb-4">Nuestros Artistas Destacados</h2>
      <div class="row">
        <div class="col-md-4 mb-4">
          <div class="card h-100">
            <img
              src="../assets/img/per-1.png"
              class="card-img-top"
              alt="imagen"
            />
            <Artista
              nombre="María Pérez"
              edad="Edad: 28 años"
              descripcion="Conoció nuestra página mientras buscaba nuevas oportunidades para promocionar su música."
            ></Artista>
          </div>
        </div>
        <div class="col-md-4 mb-4">
          <div class="card h-100">
            <img
              src="../assets/img/per-2.png"
              class="card-img-top"
              alt="imagen"
            />
            <Artista
              nombre="Juan Rodríguez"
              edad="Edad: 32 años"
              descripcion="Descubrió nuestra plataforma a través de un amigo que le recomendó distribuir su música aquí."
            ></Artista>
          </div>
        </div>
        <div class="col-md-4 mb-4">
          <div class="card h-100">
            <img
              src="../assets/img/per-3.png"
              class="card-img-top"
              alt="imagen"
            />
            <Artista
              nombre="Ana Gutiérrez"
              edad="Edad: 30 años"
              descripcion="Se unió a nuestra comunidad después de ver una publicación en redes sociales sobre cómo promocionar su música de forma independiente."
            ></Artista>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
