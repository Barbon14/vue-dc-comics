<template>
  <div id="app">
      <AppHeader/>
      <Jumbotron/>
      <main>
        <!-- contenuto pagina -->
        <Cards/>
      </main>
      <AppFooter/>
    </div>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
import Jumbotron from '@/components/Jumbotron.vue';
import Cards from '@/components/Cards.vue';
import AppFooter from '@/components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    Jumbotron,
    Cards,
    AppFooter
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
