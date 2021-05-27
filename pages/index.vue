<template>
  <div>
    <Nav/>
    <div class="container">
      <Hero/>
      <LargeCardDisplay
        v-for="cardInfo in largeCardSections"
        :key="cardInfo.id"
        :cards-section="cardInfo"
      />
    </div>
  </div>
</template>

<script>
import { largeCardSections } from '@/assets/data.js'

export default {
  data () {
    return {
      largeCardSections
    }
  }
}
</script>

<style>
</style>
