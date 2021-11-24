<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="">
    <ul>
        <li v-for="link, i in links" :key="i" :class="link.here ? 'active' : null">
            <a :href="link.href">{{link.name}}</a>
        </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      links: [
        {
          'name' : 'CHARACTERS',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'COMICS',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'MOVIES',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'TV',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'GAMES',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'COLLECTIBLES',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'VIDEOS',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'FANS',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'NEWS',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'SHOP',
          'here' : true,
          'href' : '#'
        },{
          'name' : 'NEWS',
          'here' : true,
          'href' : '#'
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;

  ul {
    display: flex;
    list-style: none;
    
    li {
      margin: 0 10px;

      a {
        text-decoration: none;
        color: #464646;
      }
    }
  }
}
</style>