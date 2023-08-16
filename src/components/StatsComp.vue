<template>
  <section class="flexCenter flex-row flex-wrap sm:mb-20 mb-6 wrapper">
    <div
      v-for="stat in stats"
      :key="stat.id"
      class="flex-1 flex justify-start items-center m-2 sm:border-r last:border-none pr-3"
    >
      <h4
        class="font-poppins font-semibold xs:text-[38px] text-[28px] xs:leading[53px] leading-[43px] text-white"
      >
        {{ stat.value }}
      </h4>
      <p
        class="font-poppins font-normal xs:text-[18px] text-[13px] xs:leading[26px] leading-[21px] text-gradient uppercase ml-3"
      >
        {{ stat.title }}
      </p>
    </div>
  </section>
</template>

<script setup>
import { stats } from '../constants'
</script>

<style lang="scss" scoped></style>
