<template>
    <div>
      <div  class="pill-container">
        <div class="pill" v-for="(pill, index) in img_names" :key="index"></div>
      </div>  
    </div>
</template>
<script>
export default {
    data() {
      return {
        img_names:['img.png','img1.png','img2.jpg']
      }
    },
}
</script>
<style >
    .pill-container{
      width: min(90%,1200px);
      margin: 0 auto;
      /* background-color: springgreen; */
      height: 70vh;
      margin-block: 2rem;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
    }
    .pill{
      height: 70vh;
      width: 20vw;
      background-color: #101c1c;
      border-radius: 200px;
      position: absolute;
    }

    img{
      width: 100%;
      height: 100%;
object-fit: cover;
    }

    .pill:nth-child(1){
      /* background-color: red; */
      left: 15%;
      border-color: red;
      background-image: url('../images/img1.png');
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
      /* padding: 1rem; */
    }
    .pill:nth-child(2){
      /* background-color: yellow; */
      /* padding: 1rem; */
      z-index: -1;
      background-image: url('../images/img2.jpg');
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
    }
    .pill:nth-child(3){
      right: 15%;
      background-image: url('../images/img.png');
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
      /* padding: 1rem; */
      background-color: transparent;
     border: 1px solid rgb(255, 255, 255);
     border-top-color: transparent;
     border-left-color: transparent;
     border-right-color: transparent;
    }
</style>