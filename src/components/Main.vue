<template>
    <div class="main-background">
        <div class="centered-container">
            <div class="main-list">                               
                <ul>
                    <li><h4>DC COMICS</h4></li>
                    <li v-for="(comics, index) in MainDcComicsList" :key="index">{{comics.text}}</li>
                </ul>                                  
                <ul>
                    <li><h4>SHOP</h4></li>
                    <li v-for="(shop, index) in MainShopList" :key="index">{{shop.text}}</li>
                </ul>                                              
                <ul>
                    <li><h4>DC</h4></li>
                    <li v-for="(dc, index) in MainDcList" :key="index">{{dc.text}}</li>
                </ul>  
                <ul>
                    <li><h4>SITES</h4></li>
                    <li v-for="(sites, index) in MainSitesList" :key="index">{{sites.text}}</li>
                </ul>            
            </div>
            <div class="logo-list">
            <img src="../assets/images/dc-logo-bg.png" alt="">
        </div>
        </div>         
    </div>
</template>

<script>
export default {
name: 'IndexMain',
data: function(){
    return{
    MainDcComicsList : [
    {
    title: "DC COMICS"
    },
    {
    text:"Characters",
    url : "#",
    },
    {
    text:"Comics",
    url : "#",
    },
    {
    text:"Movies",
    url : "#",
    },
    {
    text:"TV",
    url : "#",
    },
    {
    text:"Games",
    url : "#",
    },
    {
    text:"Videos",
    url : "#",
    },
    {
    text:"News",
    url : "#",
    },
    ],
    MainShopList : [
    {
    title: "SHOP"
    },
    {
    text: "Shop DC",
    url : "#",
    },
    {
    text:"Shop DC Collectibles",
    url : "#",
    },
    ],
    MainDcList : [
    {
    title: "DC"
    },
    {
    text:"Terms Of Use",
    url : "#",
    },
    {
    text:"Privacy policy (New)",
    url : "#",
    },
    {
    text:"Ad Choices",
    url : "#",
    },
    {
    text:"Advertising",
    url : "#",
    },
    {
    text:"Jobs",
    url : "#",
    },
    {
    text:"Subscriptions",
    url : "#",
    },
    {
    text:"Talent Workshops",
    url : "#",
    },
    {
    text:"CPSC Certificates",
    url : "#",
    },
    {
    text:"Ratings",
    url : "#",
    },
    {
    text:"Shop Help",
    url : "#",
    },
    {
    text:"Contact us",
    url : "#",
    },
],
MainSitesList : [
    {
    title: "SHOP"
    },
    {
    text: "DC",
    url : "#",
    },
    {
    text:"MAD Magazine",
    url : "#",
    },
    {
    text: "DC Kids",
    url : "#",
    },
    {
    text: "DC Universe",
    url : "#",
    },
    {
    text: "DC Power Visa",
    url : "#",
    },
    ],    
}
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
ul{
    list-style-type: none;
    color: rgb(173, 172, 172);
}
li{
    margin-bottom: .2rem;
}
h4{
    color: white;
    margin-bottom: .8rem;
}
div.main-background{
    background-image: url(../assets/images/footer-bg.jpg);
    border: 2px solid black;
}
div.centered-container{
    display: flex;
    justify-content: space-between;
    border: 2px solid green;
    width: 80%;
    height: 100%;
    margin: 0 auto;
    }
div.main-list{
    border: 2px solid gold;
    width: 60%;
    display: flex;
    justify-content: space-around;
    
}    
div.logo-list{
    border: 2px solid red;
    width: 40%;
}
div.logo-list img{ 
    width: 200px;
}    
</style>
