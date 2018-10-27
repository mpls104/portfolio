<template>
<div>
    <section class="hero is-medium is-light is-bold">
    <div class="hero-body">
      <div class="container">
        <h1 class="title">
          Welcome to myportfolio.
        </h1>
      </div>
    </div>
  </section>

  <works />
</div>
</template>

<script>
import Works from '~/components/Works.vue'
export default {
  components: {
    Works
  },
  head: {
    title: 'Home'
  }
}
</script>
