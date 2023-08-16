<template>
  <section class="section wrapper">
    <div class="sectionInfo">
      <h2 class="heading2">
        Find a better card deal <br class="sm:block hidden" />
        in a few days.
      </h2>
      <p class="paragraph max-w-[480px] mt-5">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Delectus, voluptatem!
      </p>
      <ButtonComp :style="'mt-10'" text="Get Started"></ButtonComp>
    </div>

    <div class="sectionImg">
      <img :src="card" alt="card" class="w-full h-full" />
    </div>
  </section>
</template>

<script setup>
import { card } from '../assets'
import ButtonComp from './ButtonComp.vue'
</script>

<style lang="scss" scoped></style>
