<template>
  <div
    class="flex flex-row p-6 rounded-[20px] mb-6 last:mb-0 feature-card cursor-pointer transition-all duration-150 ease-linear"
  >
    <div class="w-[64px] h-[64px] rounded-full flexCenter bg-dimBlue">
      <img :src="feature.icon" alt="icon" class="w-[50%] h-[50%] object-contain" />
    </div>
    <div class="flex-1 flex flex-col ml-3">
      <h4 class="font-poppins font-semibold text-white text-[18px] leading-[23px] mb-1">
        {{ feature.title }}
      </h4>
      <p class="font-poppins font-normal text-dimWhite text-[16px] leading-[24px] mb-1">
        {{ feature.content }}
      </p>
    </div>
  </div>
</template>

<script setup>
defineProps(['feature', 'index'])
</script>

<style lang="scss" scoped></style>
