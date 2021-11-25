<template>
  <div>
    <Navbar />
    <Main />
    <Footer />
    <Current />

    <div />

  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import Current from './components/Current.vue'



export default {
  name: 'App',
  components: {
    Navbar,
    Main,
    Footer,
    Current,
  },
  methods:{

  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
