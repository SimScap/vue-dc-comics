<template>
    <div class="blue-banner">
        <div class="blue-banner-container">
        <div class="banner-list" v-for="(link, index) in BannerNavList" :key="index">
            <img :src="'./images/' + link.imgName" :alt="link.text + 'image'">
            <span>{{link.text}}</span>
        </div>
    </div>
    </div>
</template>

<script>
export default {
name: 'IndexBanner',
data: function(){
    return{
    BannerNavList : [
    {
    text:"DIGITAL COMICS",
    url : "#",
    imgName :"buy-comics-digital-comics.png",
    },
    {
    text:"DC MERCHANDISE",
    url : "#",
    imgName :"buy-comics-merchandise.png",
    },
    {
    text:"SUBSCRIPTION",
    url : "#",
    imgName :"buy-comics-subscriptions.png",
    },
    {
    text:"COMIC SHOP LOCATOR",
    url : "#",
    imgName :"buy-comics-shop-locator.png",
    },
    {
    text:"DC POWER VISA",
    url : "#",
    imgName :"buy-dc-power-visa.svg",
    },
    ]
}
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
div.blue-banner{
    height: 120px;
    background-color:rgb(2, 130, 249) ;
div.blue-banner-container{
    display: flex;
    border: 2px solid green;
    width: 80%;
    margin: 0 auto;
    height: 120px;
    padding: 1rem;
    justify-content: space-around;
}
}
div.banner-list{
    border: 2px solid gold;
    display: flex;
}
div.banner-list img{
    width: 60px;
}
div.banner-list span{
    align-self: center;
    font-size: .8rem;
}
</style>
