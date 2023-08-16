<template>
  <section
    id="home"
    :class="`${styles.paddingY}`"
    class="flex md:flex-row flex-col wrapper mx-auto"
  >
    <div :class="`${styles.flexStart} flex-1 flex-col py-6 items-start`" class="">
      <div
        class="flex flex-row items-center py-[6px] px-5 bg-discount-gradient rounded-[10px] mb-2 text-dimWhite"
      >
        <img :src="discount" alt="discount" class="w-[32px] h-[32px]" />
        <p class="ml-2" :class="styles.paragraph">
          <span class="text-white">20% </span> Discount for
          <span class="text-white"> 1 Month</span> Account
        </p>
      </div>
      <div
        class="flex flex-row justify-between items-center w-full pr-5 ss:pr-0 sm:pr-[55px] lg:pr-0"
      >
        <h1
          class="flex-1 font-poppins font-bold ss:text-[72px] text-[52px] text-white ss:leading-[100px] leading-[75px]"
        >
          The Next <br class="sm:block hidden" />
          <span class="text-gradient">Generation</span>
        </h1>
        <div class="ss:flex hidden md:mr-4 mr-0">
          <GetStarted />
        </div>
      </div>

      <h1
        class="font-poppins font-bold ss:text-[68px] text-[52px] text-white ss:leading-[100px] leading-[75px] w-full"
      >
        Payment Method.
      </h1>

      <p :class="`${styles.paragraph} max-w-[470px] mt-5 pr-5 ss:pr-0`">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid pariatur sint quo? Ab,
        quos. Sit optio aliquam distinctio maiores numquam!
      </p>
    </div>

    <div class="relative flex-1 flex md:my-0 my-10 -mr-10 ss:-mr-36">
      <img :src="robot" alt="billing" class="w-full h-full relative z-10" />
      <div class="absolute z-0 w-[40%] h-[35%] top-0 pink__gradient"></div>
      <div class="absolute z-[1] w-[80%] h-[80%] rounded-full bottom-[40] white__gradient"></div>
      <div class="absolute z-0 w-[50%] h-[50%] top-0 right-20 blue__gradient"></div>
    </div>
    <div :class="`${styles.flexCenter} ss:hidden`">
      <GetStarted />
    </div>
  </section>
</template>

<script setup>
import { GetStarted } from './index'
import { discount, robot } from '../assets'
import { styles } from '../constants/styles'
</script>

<style lang="scss" scoped></style>
