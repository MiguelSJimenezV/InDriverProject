<script setup>
import Artista from "./Artista.vue";
import temas from "../assets/js/temas.json";
import Lanzamiento from "./Launcher.vue";
</script>
<template>
  <section class="py-5">
    <div class="container">
      <Lanzamiento
        title="Lanzamientos en vivo"
        msg="Los lanzamientos que se muestran aquí ya están disponibles en los
      servicios de música (si elegiste una fecha de lanzamiento durante la
      carga) o están a la espera de salir una vez que las tiendas hayan
      terminado de procesarlos. Haz clic en un lanzamiento para ver más
      detalles."
      ></Lanzamiento>
      <div class="row">
        <div class="col-md-3 mb-3" v-for="item in temas">
          <Artista
            v-show="item.aprobada"
            :title="item.title"
            :artista="item.artista"
            :anio="item.anio"
            :genero="item.genero"
            :tipo="item.tipo"
            class="bg-dark text-light p-3 text-center"
          ></Artista>
        </div>
      </div>
    </div>
  </section>
</template>
