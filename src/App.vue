<template>
  <div id="app">
      <Header/>
      <Jumbotron/>
      <main>
        <!-- contenuto pagina -->
        <Cards/>
      </main>
      <Footer/>
    </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Jumbotron from '@/components/Jumbotron.vue';
import Cards from '@/components/Cards.vue';
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Cards,
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
