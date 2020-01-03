<template>
  <div id="app">
    <section class="hero is-primary is-medium">
      <router-view></router-view>
      <div class="hero-foot">
        <div class="columns is-mobile">
          <Movie v-for="movieChoice in movieChoices" :movieChoice="movieChoice" :key="movieChoices.indexOf(movieChoice)"></Movie>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import Movie from './components/MovieSection'
import movieChoices from './data/movie'

export default {
    name: 'app',
    data() {
        return {
            movieChoices
        }
    },
    components: {
        Movie : Movie
    },
}
</script>

<style lang="scss" src="./assets/styles/app.scss">

</style>
