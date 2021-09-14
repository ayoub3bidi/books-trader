<template>
  <div>
    <Nav />
    <div class="container">
      <LargeCardDisplay
        v-for="cardInfo in largeCardInfo.slice(0,1)"
        :key="cardInfo.id"
        :info="cardInfo"
      />
      <Footer />
    </div>
  </div>
</template>

<script>
import { largeCardSections } from '@/assets/data.js'

export default {
  data () {
    return {
      largeCardInfo: largeCardSections
    }
  }
}
</script>
