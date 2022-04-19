<template>
  <div id="app">
    <TweetSelection/>
  </div>
</template>

<script>
import TweetSelection from './components/TweetSelection.vue'

export default {
  name: 'App',
  components: {
    TweetSelection
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
