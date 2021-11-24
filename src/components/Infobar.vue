<template>
  <section>
    <div class="box">
      <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      <p class="description">digital comics</p>
    </div>
    <div class="box">
      <img src="../assets/img/buy-comics-merchandise.png" alt="">
      <p class="description">dc merchandise</p>
    </div>
    <div class="box">
      <img src="../assets/img/buy-comics-subscriptions.png" alt="">
      <p class="description">subscription</p>
    </div>
    <div class="box">
      <img src="../assets/img/buy-comics-shop-locator.png" alt="">
      <p class="description">comic shop locator</p>
    </div>
    <div class="box">
      <img src="../assets/img/buy-dc-power-visa.svg" alt="">
      <p class="description">dc power visa</p>
    </div>
  </section>
</template>

<script>
export default {
  name:'Infobar'
}
</script>

<style lang='scss'>
section{
  display: flex;
  justify-content: center;
  padding: 30px 0;
  background-color: #0282F9;
  
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