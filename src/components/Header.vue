<template>
    <div class="centered-container">
      <div class="header-img-container">
        <img src="../assets/images/dc-logo.png" alt="">
      </div>    
      <nav class="header-nav">
        <ul>
          <li>CHARACTERS</li>
          <li>COMICS</li>
          <li>MOVIES</li>
          <li>TV</li>
          <li>GAMES</li>
          <li>COLLECTIBLES</li>
          <li>VIDEOS</li>
          <li>FANS</li>
          <li>NEWS</li>
          <li>SHOP</li>
        </ul>
      </nav>
    </div>   
</template>

<script>
export default {
  name: 'IndexHeader',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";

  div.centered-container{
    display: flex;
    justify-content: space-between;
    border: 2px solid green;
    width: 80%;
    margin: 0 auto;
    height: 100px;
  div.header-img-container{
    border: 2px solid chocolate;
    display: flex;
  }
  nav.header-nav{
    border: 2px solid magenta;
    width: 70%;
  }
  nav.header-nav ul{
    display: flex;
    list-style-type: none;
    justify-content: space-around;
    height: 100%;
  }
  nav.header-nav ul li{
    align-self: center;
  
  }
  }
</style>
