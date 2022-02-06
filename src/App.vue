<template>
  <ErrorPage/>
</template>

<script>
import ErrorPage from './components/ErrorPage.vue'

export default {
  name: 'App',
  components: {
    ErrorPage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
