<template>
  <div id="app">
      <Header/>
      <Jumbotron/>
      <main>
        <!-- contenuto pagina -->
      </main>
      <Footer/>
    </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Jumbotron from '@/components/Jumbotron.vue';
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Footer
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

#app {
  font-family: sans-serif;
}

.container {
  width: 70%;
  margin: 0 auto;
  height: 100%;
}
</style>
