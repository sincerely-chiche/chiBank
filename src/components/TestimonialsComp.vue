<template>
  <section id="clients" class="wrapper paddingY flexCenter flex-col relative">
    <div class="absolute z-0 h-[60%] w-[60%] -right-[50%] rounded-full blue__gradient" />

    <div
      class="w-full flex justify-between items-center md:flex-row flex-col sm:mb-16 mb-6 relative z-10"
    >
      <h1 class="heading2">
        What people are <br class="sm:block hidden" />
        saying about us
      </h1>

      <div class="w-full md:mt-0 mt-6">
        <p class="paragraph text-right max-w-[450px]">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reprehenderit, similique?
        </p>
      </div>
    </div>

    <div
      class="flex flex-wrap sm:justify-start justify-center w-full feedback-container relative z-10"
    >
      <FeedbackComp v-for="(feedback, index) in feedbacks" :key="index" :feedback="feedback" />
    </div>
  </section>
</template>

<script setup>
import { feedbacks } from '../constants'
import FeedbackComp from './FeedbackComp.vue'
</script>

<style lang="scss" scoped></style>
