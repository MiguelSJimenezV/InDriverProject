<script setup>
import Artista from "./Artista.vue";
import Lanzamiento from "./Launcher.vue";
import temas from "../assets/js/temas.json";
</script>
<template>
  <div class="bg-dark">
    <section class="p-3">
      <div class="container">
        <div
          class="card p-4 bg-secondary mb-12 text-light flex flex-col items-start"
        >
          <p class="text-title-large mb-2">
            ¿Tu música aún no está lista? Masteriza tus canciones para hacerlas
            sonar perfectas.
          </p>
          <a
            href="/upload"
            class="text-warning text-decoration-none fs-3 fw-bold"
          >
            Masteriza tu música
          </a>
          <p
            class="flex justify-center text-body-small text-on-surface-muted-2 mt-2"
          >
            Patrocinado por Spotify for Artists
          </p>
        </div>
      </div>
    </section>

    <section class="py-5">
      <div class="container text-light">
        <Lanzamiento
          title="En Curso"
          msg="Los lanzamientos que se muestran aquí están en curso y están a la
          espera de revisión, se están revisando actualmente o se han entregado
          a las tiendas que esperan su lanzamiento en la fecha de lanzamiento."
        ></Lanzamiento>
        <div class="row">
          <div class="col-md-3 mb-3" v-for="item in temas">
            <Artista
              v-show="!item.aprobada"
              :title="item.title"
              :artista="item.artista"
              :anio="item.anio"
              :genero="item.genero"
              :tipo="item.tipo"
              class="p-3 text-center"
            ></Artista>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
