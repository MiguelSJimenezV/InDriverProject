<script setup>
import FormBody from "./FormBody.vue";
</script>
<template>
  <div class="py-2 container">
    <div
      class="row content-center d-flex justify-content-center align-items-center my-2 p-3"
    >
      <div class="p-5 card">
        <h2>¡Contáctanos!</h2>
        <p>
          Estamos aquí para ayudarte. Completa el formulario a continuación y
          nos pondremos en contacto contigo lo antes posible.
        </p>
        <form
          action=""
          method="get"
          class="formulario"
          onsubmit="vGenerales(event)"
        >
          <FormBody></FormBody>
        </form>
      </div>
    </div>
  </div>
</template>

<style>
.hform {
  max-height: 100%;
  height: 6rem;
}
</style>
