<template>
  <section
    class="paddingY wrapper flexCenter marginY sm:flex-row flex-col bg-black-gradient-2 rounded-lg box-shadow"
  >
    <div class="flex-1 flex flex-col">
      <h2 class="heading2">Let's try our service now!</h2>
      <p class="max-w-[470px] paragraph mt-5">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Error omnis velit ipsum atque
        neque? Delectus voluptas laboriosam unde cum alias.
      </p>
    </div>
    <div class="flexCenter sm:ml-10 ml-0 sm:mt-0 mt-10">
      <ButtonComp text="Get Started"></ButtonComp>
    </div>
  </section>
</template>

<script setup>
import ButtonComp from './ButtonComp.vue'
</script>

<style lang="scss" scoped></style>
