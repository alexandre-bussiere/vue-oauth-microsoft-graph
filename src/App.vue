<template>
  <div id="app">
    <base-header />
    <HomePage />
    <base-footer />
  </div>
</template>

<script>
import HomePage from './pages/HomePage.vue'
import BaseHeader from './components/base_header.vue'
import BaseFooter from './components/base_footer.vue'

export default {
  name: 'App',
  components: {
    HomePage,
    BaseHeader,
    BaseFooter
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  margin-top: 60px;
}
</style>
