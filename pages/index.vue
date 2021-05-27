<template>
  <div>
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
import { largeCardSections } from 'assets/../assets/data'

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
