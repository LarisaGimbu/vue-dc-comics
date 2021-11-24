<template>
  <header class="container">
    <img src="../assets/img/dc-logo.png" alt="logo">
    <nav>
      <ul>
        <li>characters</li>
        <li>comics</li>
        <li>movies</li>
        <li>tv</li>
        <li>games</li>
        <li>collectbles</li>
        <li>videos</li>
        <li>fans</li>
        <li>news</li>
        <li>shop</li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name:'Header'
}
</script>

<style lang='scss'>
header{
  display: flex;
  justify-content: space-between;
  height: 100px;
  ul{
    list-style: none;
    li{
      display: inline-block;
      padding-right: 1rem;
      text-transform: uppercase;
      font-size: 0.9rem;
      font-weight: bold;
      line-height: 100px;
      color: #464646;
    }

  }
  
}
</style>