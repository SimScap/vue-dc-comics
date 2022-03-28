<template>
<div>
    <div class="centered-container">
      <div class="header-img-container">
        <img src="../assets/images/dc-logo.png" alt="dc-logo-header">
      </div>    
      <nav class="header-nav">
        <ul>
          <li v-for="(link, index) in headerNavList" :key="index">
            <a href="link.url">{{link.text}}</a>
          </li>        
        </ul>
      </nav>
    </div>
    <div class="content-goes">
      <div class="centered-container">
        <h3>..Content Goes Here..</h3>
      </div>
    </div>
</div>
</template>

<script>
export default {
  name: 'IndexHeader',
  data: function(){
    return{
      headerNavList : [
        {
        text:"CHARACTERS",
        url : "#",
      },
       {
        text:"COMICS",
        url : "#",
      },
       {
        text:"MOVIES",
        url : "#",
      },
       {
        text:"TV",
        url : "#",
      },
       {
        text:"GAMES",
        url : "#",
      },
       {
        text:"COLLECTIBLES",
        url : "#",
      },
       {
        text:"VIDEOS",
        url : "#",
      },
       {
        text:"FANS",
        url : "#",
      },
       {
        text:"NEWS",
        url : "#",
      },
       {
        text:"SHOP",
        url : "#",
      },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";
  a{
    text-decoration: none;
    
  }
  h3{
    color: white;
    align-self: center;
  }
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
  div.header-img-container img{
    padding: .8rem;
  }
  nav.header-nav{
    border: 2px solid magenta;
    width: 80%;
  }
  nav.header-nav ul{
    display: flex;
    list-style-type: none;
    justify-content: space-around;
    height: 100%;
  }
  nav.header-nav ul li{
    align-self: center;
    font-size: .8rem;
  }
  }
  div.content-goes{
    background-color: black;
    height: 100px;
  }
</style>
