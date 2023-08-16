<template>
  <div
    class="text-white"
    :class="`${styles.flexCenter}
      w-[140px] h-[140px] rounded-full bg-blue-gradient p-0.5 cursor-pointer mx-auto ss:mx-0
    `"
  >
    <div
      :class="`${styles.flexCenter} flex flex-col items-center justify-center bg-primary w-full h-full rounded-full`"
    >
      <div :class="`${styles.flexStart} flex-row`">
        <p class="font-poppins font-medium text-[18px] leading-[23px] mr-2">
          <span class="text-gradient">Get</span>
        </p>
        <img :src="arrowUp" alt="Arrow" class="w-[23px] h-[23px] object-contain" />
      </div>
      <p class="font-poppins font-medium text-[18px] leading-[23px]">
        <span class="text-gradient">Started</span>
      </p>
    </div>
  </div>
</template>

<script setup>
import { arrowUp } from '../assets'
import { styles } from '../constants/styles'
</script>

<style lang="scss" scoped></style>
