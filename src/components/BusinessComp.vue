<template>
  <section id="features" class="section wrapper">
    <div class="sectionInfo">
      <h2 class="heading2">
        You do the business, we'll <br class="sm:block hidden" />
        handle the money.
      </h2>
      <p class="paragraph max-w-[470px] mt-5">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident voluptatem odit iste in,
        fugit exercitationem? Accusantium modi adipisci obcaecati quia.
      </p>

      <ButtonComp :style="'mt-10'" :text="'Get Started'" />
    </div>

    <div class="sectionImg flex flex-col">
      <FeatureCardComp
        v-for="(feature, index) in features"
        :key="index"
        :feature="feature"
        :index="index"
      />
    </div>
  </section>
</template>

<script setup>
import { features } from '../constants'
import ButtonComp from './ButtonComp.vue'
import FeatureCardComp from './FeatureCardComp.vue'
</script>

<style lang="scss" scoped></style>
