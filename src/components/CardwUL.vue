<script setup>
import mision from "../assets/js/mision.json";

defineProps({
  title: {
    type: String,
    required: true,
  },
  msg: {
    type: String,
    required: true,
  },
});
</script>
<template>
  <div class="col-md-6" v-for="item in mision">
    <div class="card bg-secondary p-4 text-light h-100">
      <div class="h-100 mb-2">
        <h4 class="text-center">{{ item.title }}</h4>
        <p>
          {{ item.msg }}
        </p>
      </div>
      <div class="h-100">
        <ul>
          <li v-for="items in item.ul">{{ items }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>
