<template>
  <main>
    <div class="jumbotron">
      <div class="btn">current series</div>
    </div>
    <div class="container">
      <Cards 
      v-for="(serie, index) in seriesData" 
      :key="index"
      :image="serie.thumb"
      :text="serie.series"/>
      
      <div class="btn">load more</div>
      
    </div>
  </main>
</template>

<script>
import Cards from './Cards.vue';
import seriesData from '../assets/data/seriesData.js';

export default {
  name: 'Main',
  components:{
    Cards
  },
  data(){
    return{
      seriesData,
    }
  }
}
</script>

<style lang='scss'>
main{
  background-color: #1C1C1C;
  .jumbotron{
    position: relative;
    background-image: url('../assets/img/jumbotron.jpg');
    height: 300px;
    background-size: cover;
    .btn{
      position: absolute;
      left: 100px;
      top: 94%;
      width: 160px;
      font-weight: bold;
      font-size: 1.1rem;
    }
  }
  .container{
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    
    .btn{
      margin: 30px 0 20px 0;
      width: 150px;
      text-align: center;
      font-size: 0.9rem;
    }
  }
}
</style>