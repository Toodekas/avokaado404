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
  font-family: "MuseoSans", sans-serif !important;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
