<template>
  <NuxtLink :to="`/products/${card.id}`" class="card">
    <img class="image" :src="card.image">
    <h3 class="header">
      {{ card.title }}
    </h3>
    <p class="snippet">
      {{ card.snippet }}
    </p>
  </NuxtLink>
</template>

<script>
export default {
  props: ['card']
}
</script>

<style scoped>
    .card {
        width: 31.5%;
        height: auto;
        border: none;
        overflow: hidden;
        padding: 0;
        cursor: pointer;
    }
    .image {
        height: auto;
        width: 50%;
        border-radius: 0.5rem;
    }
    .header {
        font-size: 1.15rem;
        margin-top: 0.4rem;
        color: black;
    }
    .header:hover {
      color: black;
      text-decoration: none;
    }
    .snippet {
        color: grey
    }
    a:link { text-decoration: none; }
    a:visited { text-decoration: none; }
    a:hover { text-decoration: none; }
    a:active { text-decoration: none; }
</style>
