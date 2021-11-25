<template>
  <div class="box">
    <div class="image-box">
      <img :src="image">
    </div>
    <p>{{text}}</p>
  </div>
</template>

<script>
export default {
  name: 'Cards',
  props:{
    image: String,
    text: String
  }
}
</script>

<style lang="scss">
.box{
  margin-top: 40px;
  margin-right: 20px;
  width: 140px;
  &:hover{
    cursor: pointer;
    box-shadow: 1px 1px 5px white;
  }
  .image-box{
    width: 100%;
    height: 140px;
    overflow: hidden;
    img{
      width: 100%;
    }
  }
  p{
    color: white;
    text-transform: uppercase;
    padding-top: 10px;
    font-size: 0.7rem;
  }
}
</style>