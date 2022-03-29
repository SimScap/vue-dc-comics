<template>
    <div class="footer-background">
        <div class="footer-wrap">
            <div class="footer-btn">
            <button>SIGN-UP NOW!</button>
        </div>
        <div class="footer-nav">
            <a href="#">FOLLOW US</a>
            <ul>
                <li v-for="(link, index) in FooterList" :key="index">
                    <img :src="'./images/' + link.imgName" :alt="link.text + 'image'">
                </li>               
            </ul>
        </div>
        </div>
    </div>
</template>

<script>
export default {
name: 'IndexHeader',
data: function(){
    return{
    FooterList : [
    {
    imgName :"footer-facebook.png",
    },
    {
    imgName :"footer-twitter.png",
    },
    {
    imgName :"footer-youtube.png",
    },
    {
    imgName :"footer-pinterest.png",
    },
    {
    imgName :"footer-periscope.png",
    },
    ]
}
}
}

</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
a{
    align-self: center;
    text-decoration: none;
}
ul{
    list-style-type: none;
    display: flex;
    width: 80%;
    justify-content: flex-end;
}
li{
    align-self: center;
    margin-left: .8rem;
}
div.footer-background{
    background-color: rgb(48, 48, 48);
    height: 100px;
}
div.footer-wrap{
    display: flex;
    justify-content: space-between;
    border: 2px solid green;
    width: 80%;
    height: 100%;
    margin: 0 auto;
}
div.footer-btn{
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 30%;
    border: 2px solid brown;
    padding: .8rem;
}
div.footer-btn button{
    width: 120px;
    border: 2px solid blue;
    background-color: rgb(48, 48, 48);
    color: white;
    padding: .5rem;
}
div.footer-nav{
    display: flex;
    justify-content: space-between;
    width: 40%;
    border: 2px solid blue;
    padding: .5rem;
}
</style>
