<script setup>
import SimpleCard from "./SimpleCard.vue";
</script>
<template>
  <section class="bg-light py-5" id="equipo">
    <div class="container">
      <h2 class="text-center mb-4">Nuestro Equipo</h2>
      <div class="row">
        <div class="col-md-4 py-3">
          <div class="text-center">
            <img
              src="../assets/img/equipo-1.jpg"
              alt="Foto de usuario"
              class="rounded-circle mb-3"
            />
          </div>
          <SimpleCard title="Juan Pérez" msg="Director Ejecutivo" class="">
          </SimpleCard>
        </div>
        <div class="col-md-4 py-3">
          <div class="text-center">
            <img
              src="../assets/img/equipo-2.jpg"
              alt="Foto de usuario"
              class="rounded-circle mb-3"
            />
          </div>
          <SimpleCard title="Carlos Rodríguez" msg="Desarrollador Web" class="">
          </SimpleCard>
        </div>
        <div class="col-md-4 py-3">
          <div class="text-center">
            <img
              src="../assets/img/equipo-3.jpg"
              alt="Foto de usuario"
              class="rounded-circle mb-3"
            />
          </div>
          <SimpleCard title="María García" msg="Gerente de Marketing" class="">
          </SimpleCard>
        </div>
        <div class="col-md-4">
          <div class="text-center">
            <img
              src="../assets/img/equipo-4.jpg"
              alt="Foto de usuario"
              class="rounded-circle mb-3"
            />
          </div>
          <SimpleCard title="Lautaro López" msg="Diseñador Gráfico" class="">
          </SimpleCard>
        </div>
        <div class="col-md-4">
          <div class="text-center">
            <img
              src="../assets/img/equipo-5.jpg"
              alt="Foto de usuario"
              class="rounded-circle mb-3"
            />
          </div>
          <SimpleCard
            title="Pedro Martínez"
            msg="Especialista en Contenidos"
            class=""
          >
          </SimpleCard>
        </div>
        <div class="col-md-4">
          <div class="text-center">
            <img
              src="../assets/img/equipo-6.jpg"
              alt="Foto de usuario"
              class="rounded-circle mb-3"
            />
          </div>
          <SimpleCard
            title="Laura Fernández"
            msg="Coordinadora de Eventos"
            class=""
          >
          </SimpleCard>
        </div>
      </div>
    </div>
  </section>
</template>
