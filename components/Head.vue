<template>
  <div class="Hero container">
    <div class="text-container">
      <h1 class="display-6">
        Let's find your Book!
      </h1>
      <p class="lead">
        Sometimes we can't find the physical book that we want in the libraries.
        That's why we provide you with <b>Books Trader</b> that will help you find what you want. <br>
        Happy reading!
      </p>
      <button class="button btn">
        Start Looking
      </button>
    </div>
    <img class="image" src="~assets/svg/undraw_Bookshelves_re_lxoy.svg" alt="Books">
  </div>
</template>

<script>
import { mapState } from 'vuex'

export default {
  conputed: {
    ...mapState
  }
}
</script>

<style scoped>
    .Hero {
        height: 50vh;
        position: relative;
        display: flex;
        padding: 5rem 0;
        align-items: flex-start;
        justify-content: space-between;
    }
    .text-container {
        width: 50%;
        margin-top: 4rem;
    }
    .image {
        width: 27.5rem;
        margin-top: 2rem;
    }
    .overlay {
        background: rgba(0, 0, 0, 0);
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
    }
    .button {
        padding: 1rem 4rem;
        border-radius: 100rem;
        background-color: #41b883;
        color: white;
        width: 20rem;
        font-weight: 700;
        transition: 0.5s;
    }
    .button:hover {
        width: 21.5rem;
    }
    @media (max-width: 500px) {
        .Hero {
            height: 40vh;
        }
    }
</style>
