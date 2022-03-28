<template>
    <div class="footer-wrap">
        <div class="footer-btn">
            <button>SIGN-UP NOW!</button>
        </div>
        <div class="footer-nav">
            <a href="#">FOLLOW US</a>
            <ul>
                <li>ff</li>
                <li>ff</li>
                <li>ff</li>
                <li>ff</li>
                <li>ff</li>
            </ul>

        </div>

    </div>
</template>

<script>
export default {
name: 'IndexHeader',
}

</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
a{
    align-self: center;
}
ul{
    list-style-type: none;
    display: flex;
    width: 80%;
    justify-content: space-evenly;
}
li{
    align-self: center;
}
div.footer-wrap{
    display: flex;
    justify-content: space-between;
    background-color: rgb(48, 48, 48);
    height: 100px;
}
div.footer-btn{
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 30%;
    border: 2px solid brown;
}
div.footer-btn button{
    width: 100px;
    align-self: center;
    border: 2px solid blue
}
div.footer-nav{
    display: flex;
    width: 50%;
    border: 2px solid blue;
}
</style>
