<template>
  <nav class="w-full flex py-6 justify-between items-center wrapper mx-auto text-white">
    <img :src="logo" alt="chiBank" srcset="" class="w-[124px] h-[32px]" />

    <ul class="list-none sm:flex hidden justify-end items-center flex-1">
      <li
        v-for="link in navLinks"
        :key="link.id"
        :class="['font-poppins cursor-pointer text-[16px] text-white mr-10 last:mr-0']"
      >
        <a :href="`#${link.title}`">{{ link.title }}</a>
      </li>
    </ul>

    <div class="sm:hidden flex flex-1 justify-end items-center">
      <img
        :src="toggleMenu ? close : menu"
        alt="Nav Menu"
        class="w-[28px] h-[28px] object-contain transition-all duration-150 ease-linear"
        @click="toggleMenu = !toggleMenu"
      />

      <div
        :class="toggleMenu ? 'flex' : 'hidden'"
        class="p-6 bg-black-gradient absolute top-20 right-0 mx-4 my-2 min-w-[140px] rounded-xl sidebar"
      >
        <ul class="list-none flex flex-col items-center flex-1">
          <li
            v-for="link in navLinks"
            :key="link.id"
            :class="['font-poppins cursor-pointer text-[16px] text-white mb-4']"
          >
            <a :href="`#${link.title}`">{{ link.title }}</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue'
import { logo, menu, close } from '../assets'
import { navLinks } from '../constants'

const toggleMenu = ref(false)
</script>

<style lang="scss" scoped></style>
