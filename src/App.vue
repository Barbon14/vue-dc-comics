<template>
  <div id="app">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <div id="container">
      <Header/>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
import Header from '@/components/Header.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    Header
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

#container {
  width: 80%;
  margin: 0 auto;
}
</style>
