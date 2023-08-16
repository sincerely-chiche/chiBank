<template>
  <section class="wrapper flexCenter flex-col paddingY">
    <div class="flexStart md:flex-row flex-col mb-8 w-full">
      <div class="flex-1 flex flex-col justify-start mr-10">
        <img :src="logo" alt="chiBank" class="w-[266px] h-[72px] object-contain" />
        <p class="paragraph mt-4 max-w-[310px]">
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sed, ullam.
        </p>
      </div>

      <div class="flex-[1.5] w-full flex flex-row justify-between flex-wrap md:mt-0 mt-10">
        <div
          v-for="links in footerLinks"
          :key="links.title"
          class="flex flex-col ss:my-0 my-4 min-w-[150px]"
        >
          <h4 class="font-poppins font-medium text-[18px] leading-[27px] text-white mb-4">
            {{ links.title }}
          </h4>
          <ul class="list-none mt-4">
            <li
              v-for="(link, index) in links.links"
              :key="index"
              class="font-poppins font-normal text-[16px] leading-[24px] text-dimWhite hover:text-secondary cursor-pointer mb-1.5 last:mb-0"
            >
              {{ link.name }}
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div
      class="flex w-full justify-between items-center md:flex-row flex-col pt-6 border-t border-t-[#3f3e45]"
    >
      <p class="font-poppins font-normal text-[18px] leading-[27px] text-white mb-4 text-center">
        2023 chiBank. All rights reserved
      </p>

      <div class="flex flex-row md:mt-0 mt-6">
        <img
          v-for="(social, index) in socialMedia"
          :src="social.icon"
          :alt="social.id"
          :key="index"
          class="w-[21px] h-[21px] object-contain cursor-pointer mr-6 last:mr-0"
        />
      </div>
    </div>
  </section>
</template>

<script setup>
import { footerLinks, socialMedia } from '../constants'
import { logo } from '../assets'
</script>

<style lang="scss" scoped></style>
