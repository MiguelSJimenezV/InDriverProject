<script setup>
import CarouselItem from "./CarouselItem.vue";
</script>
<template>
  <header class="bg-dark text-white">
    <div
      id="carouselExampleSlidesOnly"
      class="carousel slide"
      data-ride="carousel"
    >
      <div class="carousel-inner">
        <CarouselItem
          class="bg1 active"
          title="¡Sube tu Tema!"
          msg="Comparte tu  con el mundo"
          btn="Comenzar"
        ></CarouselItem>
        <CarouselItem
          class="bg2"
          title="¡Forma parte de nuestra Comunidad!"
          msg="haz que las personas conozcan tu talento"
          btn="Subir mi música"
        ></CarouselItem>
        <CarouselItem
          class="bg3"
          title="Comparte tus canciones"
          msg="Completa el formulario y unete a InDriver"
          btn="Mas Informacion"
        ></CarouselItem>

        <a
          class="carousel-control-prev"
          href="#carouselExampleSlidesOnly"
          role="button"
          data-slide="prev"
        >
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="sr-only">Anterior</span>
        </a>
        <a
          class="carousel-control-next"
          href="#carouselExampleSlidesOnly"
          role="button"
          data-slide="next"
        >
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="sr-only">Siguiente</span>
        </a>
      </div>
    </div>
  </header>
</template>

<style>
.bg1 {
  background-image: url(../assets/img/bg-1.png);
  width: 100%;
  padding: 10%;
}
.bg2 {
  background-image: url(../assets/img/bg-2.png);
  width: 100%;
  padding: 10%;
}
.bg3 {
  background-image: url(../assets/img/bg-3.png);
  width: 100%;
  padding: 10%;
}
</style>
