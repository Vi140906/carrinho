<script setup>

import { tenis } from '@/_data/tenis'

</script>

<template>

  <h1> Santo's Skate </h1>
  <div class="tenis">
    <div class="card-tenis" v-for="tenis in tenis" :key="tenis.id">
      <img :src="tenis.cover" class="tenis-capa" />
      <p class="tenis-titulo">{{ tenis.title }}</p>
      <p class="tenis-preco">{{ tenis.price }}</p>
    </div>
  </div>

</template>

<style scoped>
</style>
