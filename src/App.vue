<template>
  <div id="app">
    <h2 class="text-primary">回国机票搜索</h2>
    <div class="d-flex flex-row">
      <flight-from-usa></flight-from-usa>
      <flight-from-korea></flight-from-korea>
      <flight-from-japan></flight-from-japan>
    </div>
  </div>
</template>

<script>
import FlightFromUsa from './components/FlightFromUsa.vue'
import FlightFromKorea from './components/FlightFromKorea.vue'
import FlightFromJapan from './components/FlightFromJapan.vue'

export default {
  name: 'App',
  components: {
    FlightFromUsa,
    FlightFromKorea,
    FlightFromJapan
  },
  data () {
    return {

    }
  }
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px;
}
</style>
