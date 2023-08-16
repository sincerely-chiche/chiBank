<template>
  <button
    type="button"
    :class="style"
    class="py-4 px-6 bg-blue-gradient font-poppins font-medium text-[18px] text-primary outline-none rounded-md"
  >
    {{ text }}
  </button>
</template>

<script setup>
defineProps(['style', 'text'])
</script>

<style lang="scss" scoped></style>
