<template >
    <div>
        <div class="header-container"> 
            <div class="world-container">
                <h2>World</h2>
            </div>
            <div class="links-container">
                <a v-for="(link, index) in links" :key="index" href="#" >{{link}}</a>
            </div>
            <div class="cart-container">
                <a href="#">Cart</a>
            </div>
        </div>
    </div>
</template>
<script>
export default{
    data() {
        return {
            links:['Exhibition','Artists','Press','Shop']
        }
    },

}
</script>
<style scoped>
.header-container{
    border: 1px solid hsl(0, 0%, 70%);
/* background-color: springgreen; */
display: flex;
border-radius: 25px;
padding-inline: 20px;
width: min(50%,1200px);
margin: 0 auto;
}
.links-container{
    display: flex;
    /* background-color: darkblue; */
    width: 100%;
    justify-content: space-evenly;
    align-items: center;
}
.world-container{
    display: flex;
    /* background-color: pink; */
    width: 20%;
}
.cart-container{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 20%;
    /* background-color: darkred; */
}
*{
    color: white;
font-family: sans-serif;
}
a{
    text-decoration: none;
}
</style>