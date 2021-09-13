<template>
  <div class="container">
    <h4 class="header">
      {{ info.title }}
    </h4>
    <p class="snippet">
      {{ info.snippet }}
    </p>
  </div>
</template>

<script>
export default {
  props: ['info']
}
</script>

<style scoped>
.container {
    margin-top: 2rem;
}
    .header {
        font-weight: 700;
        font-size: 1.5rem;
    }
    .snippet {
        color: grey;
        margin-bottom: 1.5rem;
    }
    .cards-container {
        display: flex;
        justify-content: space-between;
    }
</style>
