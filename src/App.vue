<template>
  <div class="bg-primary w-full overflow-hidden">
    <div :class="[styles.paddingX, styles.flexCenter]">
      <div :class="`${styles.boxWidth}`">
        <Navbar />
      </div>
    </div>

    <div :class="['bg-primary', styles.flexStart]">
      <div :class="`${styles.boxWidth}`"><Hero /></div>
    </div>
    <div :class="['bg-primary', styles.paddingX, styles.flexStart]">
      <div :class="`${styles.boxWidth}`">
        <stats /> <Business /> <Billing /> <CardDeal /> <Testimonials /> <Clients /> <CTA />
        <Footer />
      </div>
    </div>
  </div>
</template>

<script setup>
import {
  Navbar,
  Hero,
  Billing,
  Business,
  CardDeal,
  Clients,
  CTA,
  Stats,
  Testimonials,
  Footer
} from './components'
import { styles } from './constants/styles'
</script>

<style lang="scss" scoped></style>
