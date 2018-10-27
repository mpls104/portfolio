<template>
  <section class="main-content">
    <div class="container">
      <h1 class="title has-text-centered">
        Recent Works.
      </h1>
      <div class="columns is-multiline">
        <div class="column is-half" v-for="work in works" :key="work">
          <div class="card">
           <header class="card-header">
            <p class="card-header-title">
              {{ work.title }}
            </p>
          </header>
          <div class="card-content">
            <div class="content">
              {{ work.summary }}
            </div>
          </div>
          <footer class="card-footer">
            <nuxt-link :to="`work/${work.id}`"
              class="card-footer-item" append>
              Read More
            </nuxt-link>
          </footer>
        </div>
      </div>
    </div>
  </div>
</section>
</template>

<script>
  import works from '~/works.json'
  export default {
    name: 'works',
    data () {
      return { works }
    }
  }
</script>
