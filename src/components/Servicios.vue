<script setup>
import Servicio from "./Servicio.vue";
</script>
<template>
  <section class="bg-light">
    <div class="container">
      <h2 class="text-center mb-4">Nuestros Servicios</h2>
      <div class="row">
        <div class="col-md-6 mb-4">
          <div class="card bg-dark text-white service-card">
            <img src="../assets/img/ser-1.png" class="card-img" alt="imagen" />
            <Servicio
              title="Producción Musical"
              msg="Te ayudamos a dar vida a tus ideas musicales con nuestros
                servicios de producción profesional."
              btn="Mas Informacion"
            ></Servicio>
          </div>
        </div>
        <div class="col-md-6 mb-4">
          <div class="card bg-dark text-white service-card">
            <img src="../assets/img/ser-2.png" class="card-img" alt="..." />
            <Servicio
              title="Promoción Online"
              msg="Amplifica tu alcance con nuestras estrategias de promoción
                online diseñadas para destacar tu música en la web."
              btn="Ver Mas"
            ></Servicio>
          </div>
        </div>
        <div class="col-md-6 mb-4">
          <div class="card bg-dark text-white service-card">
            <img src="../assets/img/ser-5.png" class="card-img" alt="..." />
            <Servicio
              title="Distribución Global"
              msg="Lleva tu música a nuevas audiencias en todo el mundo con nuestra
                red de distribución global."
              btn="Descubre"
            ></Servicio>
          </div>
        </div>
        <div class="col-md-6 mb-4">
          <div class="card bg-dark text-white service-card">
            <img src="../assets/img/ser-6.png" class="card-img" alt="imagen" />
            <Servicio
              title="Gestión de Derechos"
              msg="Protege tus derechos de autor y asegura tus regalías con nuestro
                servicio de gestión de derechos."
              btn="Saber Mas"
            ></Servicio>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.equal-height .card {
  height: 100%;
}
</style>
