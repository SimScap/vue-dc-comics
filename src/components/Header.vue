<template>
<div>
    <div class="centered-container">
      <div class="header-img-container">
        <img src="../assets/images/dc-logo.png" alt="dc-logo-header">
      </div>    
      <nav class="header-nav">
        <ul>
          <li v-for="(link, index) in headerNavList" :key="index" :class="{ active: link.current}">
            <a href="link.url"  >{{link.text}}</a>
          </li>        
        </ul>
      </nav>
    </div>
    <div class="my-jumbotron">
      <img src="../assets/images/jumbotron.jpg" alt="jumbotron">
    </div>
    <div class="content-goes">
      <div class="my-centered-container">
      <div class="my-card" v-for="(products, index) in headerProducts" :key="index">
        <img :src="products.thumb" alt="">
        <h4>{{products.series}}</h4>
      </div>
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
        current : false,
      },
      {
        text:"COMICS",
        url : "#",
        current : false,

      },
      {
        text:"MOVIES",
        url : "#",
        current : false,

      },
      {
        text:"TV",
        url : "#",
        current : false,

      },
      {
        text:"GAMES",
        url : "#",
        current : false,

      },
      {
        text:"COLLECTIBLES",
        url : "#",
        current : false,

      },
      {
        text:"VIDEOS",
        url : "#",
        current : false,

      },
      {
        text:"FANS",
        url : "#",
        current : false,

      },
      {
        text:"NEWS",
        url : "#",
        current : false,

      },
      {
        text:"SHOP",
        url : "#",
        current : false,

      },
      ],
  headerProducts : [
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  },
],
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
    line-height: 90px;
    &:active,
    &.active{
        border-bottom :4px solid #0282f9;
      } 
  }
  }
  div.content-goes{
    background-color: black;
  }
  div.my-jumbotron img{
    height: 250px;
    width: 100%;
  }
  div.my-card{
    width: calc(100% / 6);
    border: 2px solid red;
    color: white;
    text-align: center;
  }
  div.my-card img{
    width: 100%;
  }
  div.my-centered-container{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    border: 2px solid green;
    width: 80%;
    margin: 0 auto;
  }
</style>
