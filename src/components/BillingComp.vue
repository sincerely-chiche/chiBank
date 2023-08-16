<template>
  <section id="product" class="sectionReverse wrapper">
    <div class="sectionImgReverse">
      <img :src="bill" alt="billing" class="w-full h-full relative z-20" />
      <div class="absolute z-10 white__gradient -left-1/2 top-0 w-[50%] h-[50%] rounded-full" />
      <div class="absolute z-0 pink__gradient -left-1/2 bottom-0 w-[50%] h-[50%] rounded-full" />
    </div>
    <div class="sectionInfo">
      <h2 class="heading2">
        Easily control your <br class="sm:block hidden" />
        billing & invoicing.
      </h2>
      <p class="paragraph max-w-[470px] mt-5">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum quia quod mollitia dolore
        tempore, voluptatum ea debitis omnis delectus sit!
      </p>

      <div class="flex flex-row flex-wrap sm:mt-10 mt-6">
        <img
          :src="apple"
          alt="apple_store"
          class="w-[128px] h-[42px] object-contain mr-5 cursor-pointer"
        />
        <img
          :src="google"
          alt="google_store"
          class="w-[128px] h-[42px] object-contain cursor-pointer"
        />
      </div>
    </div>
  </section>
</template>

<script setup>
import { apple, bill, google } from '../assets'
</script>

<style lang="scss" scoped></style>
