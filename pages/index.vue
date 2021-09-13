<template>
  <div>
    <Head /><br><br><br><br>
    <LargeCardDisplay
      v-for="cardInfo in largeCardInfo"
      :key="cardInfo.id"
      :info="cardInfo"
    />
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
