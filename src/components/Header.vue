<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="logo DC comics">
    <ul>
        <li v-for="link, i in links" :key="i" >
            <a :href="link.href" :class="link.here ? 'active' : null">
              {{link.name}}
            </a>
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
          'here' : false,
          'href' : '#'
        },
        {
          'name' : 'COMICS',
          'here' : true,
          'href' : '#'
        },
        {
          'name' : 'MOVIES',
          'here' : false,
          'href' : '#'
        },
        {
          'name' : 'TV',
          'here' : false,
          'href' : '#'
        },
        {
          'name' : 'GAMES',
          'here' : false,
          'href' : '#'
        },
        {
          'name' : 'COLLECTIBLES',
          'here' : false,
          'href' : '#'
        },
        {
          'name' : 'VIDEOS',
          'here' : false,
          'href' : '#'
        },
        {
          'name' : 'FANS',
          'here' : false,
          'href' : '#'
        },
        {
          'name' : 'NEWS',
          'here' : false,
          'href' : '#'
        },
        {
          'name' : 'SHOP',
          'here' : false,
          'href' : '#'
        },{
          'name' : 'NEWS',
          'here' : false,
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
  padding: 20px 0;

  ul {
    display: flex;
    list-style: none;
    
    li {
      margin: 0 10px;

      a {
        text-decoration: none;
        color: #464646;

        &.active{
          color: #3183fc;
        }
      }
    }
  }
}
</style>