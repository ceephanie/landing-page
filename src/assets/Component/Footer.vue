<template >
    <div class="footer-container">
        <div class="footer-start">
            <h2>
Absolutley unique body of work
            </h2>
        </div>
        <div class="footer-mid">
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Et illo voluptas facere ad recusandae nemo expedita pariatur id blanditiis ratione, reprehenderit aliquam 
            </p>
        </div>
        <div class="footer-end">
            <img src="../images/img.png" alt="">
            <img src="../images/img1.png" alt="">
            <img src="../images/img2.jpg" alt="">

        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.footer-container{
    width: min(50%, 1200px);
    margin: 0 auto;
    display: flex;
    color: white;
    font-family: sans-serif;
}
.footer-start,.footer-mid,.footer-end{
    width: 100%;

}
h2{
    width: 20ch;
}
p{
    font-size: 11px;
    line-height: 1rem;
}

.footer-end{
    display: flex;

    height: 10vh;
    justify-content: center;
    align-items: center;
    position: relative;

}
img{
    height:100%;
    width: 70px;
    border-radius: 100%;
    position: absolute;
}

img:nth-child(1){
    left:15%;
    z-index: -1;
}
img:nth-child(3){
    right:12%;
}
</style>