<template>
  <header class="container">
    <img src="../assets/img/dc-logo.png" alt="logo">
    <nav>
      <ul>
        <li 
        v-for="(item, index) in navbar" 
        :key="index"
        :class="{active: item.active}">{{item.name}}</li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name:'Header',
  data(){
    return{
      navbar:[
        {
          name: 'characters',
          active: false
        },
        {
          name: 'comics',
          active: true
        },
        {
          name: 'movies',
          active: false
        },
        {
          name: 'tv',
          active: false
        },
        {
          name: 'games',
          active: false
        },
        {
          name: 'collecatbles',
          active: false
        },
        {
          name: 'videos',
          active: false
        },
        {
          name: 'fans',
          active: false
        },
        {
          name: 'news',
          active: false
        },
        {
          name: 'shop',
          active: false
        },
      ]
    }
  }
}
</script>

<style lang='scss'>
@import '../assets/style/vars.scss';

header{
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 100px;
  img{
    width: 80px;
  }
  ul{
    list-style: none;
    li{
      display: inline-block;
      padding: 0 0.5rem;
      text-transform: uppercase;
      font-size: 0.9rem;
      font-weight: bold;
      line-height: 96px;
      color: #464646;
      &.active,
      &:hover{
        cursor: pointer;
        color: $primary-color;
        border-bottom: 4px solid $primary-color;
      }
    }

  }
  
}
</style>