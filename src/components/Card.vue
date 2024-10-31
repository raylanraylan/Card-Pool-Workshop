<script lang="ts" setup>
import { defineProps } from "vue";

defineProps<{
  imgUrl: string
}>()

</script>

<template>
  <div>
    <img v-show="imgUrl" :src="imgUrl" alt="卡片圖面"/>
  </div>
</template>

<style lang="scss" scoped>
  div {
    width: 190px;
    padding: 20px;
    border: 1px solid black;
  }

  img {
    width: 190px;
    height: 268px;
    object-fit: cover;
  }
</style>