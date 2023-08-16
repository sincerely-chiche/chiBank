<template>
  <section class="wrapper flexCenter my-4">
    <div class="flexCenter flex-wrap w-full">
      <div
        v-for="client in clients"
        :key="client.id"
        class="flex-1 flexCenter sm:min-w-[192px] min-w-[120px]"
      >
        <img :src="client.logo" alt="client" class="sm:w-[192px] w-[100px] object-contain" />
      </div>
    </div>
  </section>
</template>

<script setup>
import { clients } from '../constants'
</script>

<style lang="scss" scoped></style>
