<script setup lang="ts">
import Card from '@/components/Card.vue'
const imgUrl = new URL('@/assets/img/images.jpeg', import.meta.url).href
</script>

<template>
  <header>
  </header>

  <main>
    <div class="cards">
      <Card class="cards_card" v-for="n of 10" :style="`position:absolute;bottom:0;margin:auto;z-index:${n}`" :img-url="imgUrl"></Card>
    </div>
  </main>
</template>

<style scoped>

</style>
