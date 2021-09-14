<template>
  <div>
    <Nav />
    <div class="container">
      <Head /><br><br><br><br>
      <LargeCardDisplay
        v-for="cardInfo in largeCardInfo"
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
