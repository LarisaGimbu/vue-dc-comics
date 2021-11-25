<template>
  <section>
    <div 
    v-for="(item, index) in infobar"
    :key="index"
    class="box">
      <img :src="item.image" alt="">
      <p class="description">{{item.text}}</p>
    </div>
  </section>
</template>

<script>
export default {
  name:'Infobar',
  data(){
    return{
      infobar:[
        {
          image: require("../assets/img/buy-comics-digital-comics.png"),
          text:'digital comics'
        },
        {
          image: require("../assets/img/buy-comics-merchandise.png"),
          text:'dc merchandise'
        },
        {
          image: require("../assets/img/buy-comics-subscriptions.png"),
          text:'subscription'
        },
        {
          image: require("../assets/img/buy-comics-shop-locator.png"),
          text:'comic shop locator'
        },
        {
          image: require("../assets/img/buy-dc-power-visa.svg"),
          text:'dc power visa'
        },
      ]
    }
  }
}
</script>

<style lang='scss'>
@import '../assets/style/vars.scss';

section{
  display: flex;
  justify-content: center;
  padding: 30px 0;
  background-color: $primary-color;
  
  .box{
    display: flex;
    align-items: center;
    padding: 0 1.5rem;
    color: white;
    img{
      width: 40px;
    }
    .description{
      text-transform: uppercase;
      padding-left: 10px;
    }
  }
  
}
</style>