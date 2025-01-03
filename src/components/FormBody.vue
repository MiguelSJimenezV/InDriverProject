<script setup>
import { ref } from "vue";

defineProps({
  nombre: {
    type: String,
    required: true,
  },
  apellido: {
    type: String,
    required: true,
  },
  email: {
    type: String,
    required: true,
  },
});

let nombre = ref("");
let apellido = ref("");
let email = ref("");
let asunto = ref("");
let errorMsg = "El campo no puede quedar vacio";
let successMsg = "Campo valido";

let general = nombre && apellido && email && asunto;
let errorGral = "Verifique que todos los datos sean correctos";
let successGral =
  'Listo para enviar, presione el boton "enviar" para continuar';
</script>

<template>
  <div>
    <label for="name">Nombre</label>
    <input
      type="text"
      name="name"
      id="name"
      placeholder="Miguel"
      required
      class="form-control bg-dark text-light"
      v-model="nombre"
    />
    <div class="is-invalid text-danger p-2" v-if="!nombre">{{ errorMsg }}</div>
    <div class="is-valid text-success p-2" v-if="nombre">{{ successMsg }}</div>
  </div>

  <div>
    <label for="surname">Apellido</label>
    <input
      type="text"
      name="surname"
      id="surname"
      placeholder="Jimenez"
      required
      class="form-control bg-dark text-light"
      v-model="apellido"
    />
    <div class="is-invalid text-danger p-2" v-if="!apellido">
      {{ errorMsg }}
    </div>
    <div class="is-valid text-success p-2" v-if="apellido">
      {{ successMsg }}
    </div>
  </div>

  <div>
    <label for="email">E-mail</label>
    <input
      type="email"
      name="email"
      id="email"
      oninput=""
      required
      class="form-control bg-dark text-light"
      placeholder="Example@gmail.com"
      v-model="email"
    />
    <div class="is-invalid text-danger p-2" v-if="!email">{{ errorMsg }}</div>
    <div class="is-valid text-success p-2" v-if="email">{{ successMsg }}</div>
  </div>
  <div class="hform mb-5">
    <label for="asunto">Mensaje</label>
    <textarea
      type="text"
      name="asunto"
      id="asunto"
      placeholder="Comentanos brevemente tus dudas y te responderemos a la brevedad"
      oninput=""
      required
      class="form-control h-100 bg-dark text-light"
      v-model="asunto"
    />
    <div class="is-invalid text-danger p-2" v-if="!asunto">{{ errorMsg }}</div>
    <div class="is-valid text-success p-2" v-if="asunto">{{ successMsg }}</div>
  </div>
  <div class="py-5 px-3 row">
    <button
      id="btn"
      class=" btn btn-secondary p-3"
      type="submit"
      onclick="vGenerales(event)"
    >
      Enviar
    </button>
    <div class="is-valid text-success p-2" v-if="general">
      {{ successGral }}
    </div>
    <div class="is-invalid text-danger p-2" v-else>{{ errorGral }}</div>
  </div>
</template>
