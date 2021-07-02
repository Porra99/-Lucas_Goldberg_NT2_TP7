<template>
  <div id="app">
    <Header/>
    <Navbar/>
    <Game/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Navbar from './components/Navbar.vue'
import Game from './components/Game.vue'

export default {
  name: 'App',
  components: {
    Header,
    Navbar,
    Game,    
  },
  mounted () {
    this.$store.dispatch('restart', true)
  },
  data() {
    return{
    }
  },
  methods: {
  },

}
</script>

<style>
body {
  background: #232323;
  margin: 0;
  font-family: "Montserrat", "Avenir", serif;
}
h1 {
  font-weight: normal;
  line-height: 1.1;
  padding: 20px 0;
}
#container {
  margin: 20px auto;
  max-width: 600px;
}
</style>
