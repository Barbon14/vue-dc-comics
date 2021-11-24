<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="">
    <ul>
        <li>
            <a href="#">link</a>
        </li>
        <li>
            <a href="#">link</a>
        </li>
        <li>
            <a href="#">link</a>
        </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: 'Header'
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
      }
    }
  }
}
</style>