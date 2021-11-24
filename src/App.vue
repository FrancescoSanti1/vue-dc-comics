<template>
  <div id="app">
    <Header/>
    <main>
      <div>content goes here</div>
    </main>
    <Banner/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Banner from './components/Banner.vue';

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Banner
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

main {
  padding: 50px 0;
  background-color: black;
  color: white;
}

.container {
  width: 80%;
  margin: 0 auto;
}
</style>
