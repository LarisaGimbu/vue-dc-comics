<template>
  <footer>
    <div class="top-footer">
      <div class="container">
        <div class="left-content">
          <ul>
            <li><h3>dc comics</h3></li>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <ul>
            <li><h3>dc</h3></li>
            <li>Terms Of Use</li>
            <li>Pravacy policy (New)</li>
            <li>Ad Choice</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshops</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>
          <ul>
            <li><h3>Sites</h3></li>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>SC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>
        </div>
        <div class="right-content">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>
    <div class="bottom-footer">
      <div class="container">
        <a class="btn" href="">sign-up now!</a>
        <div class="follow-box">
          <span>FOLLOW US</span>
          <i class="fab fa-facebook-f"></i>
          <i class="fab fa-twitter"></i>
          <i class="fab fa-youtube"></i>
          <i class="fab fa-pinterest-p"></i>
          <i class="fas fa-map-marker-alt"></i>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style lang="scss">
@import '../assets/style/vars.scss';

footer{
  .top-footer{
    display: flex;
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
    overflow: hidden;
    .container{
      display: flex;
    }
    .left-content{
      display: flex;
      flex-wrap: wrap;
      width: 45%;
      padding-top: 30px;
      ul{
        list-style: none;
        padding: 20px 20px 0 0;
        li{
          color: #959595;
          font-size: 0.7rem;
          padding-bottom: 0.5rem;
          &:hover{
            color: white;
            cursor: pointer;
          }
          h3{
            font-size: 1rem;
            color: white;
            text-transform: uppercase;
            padding-bottom: 0.9rem;
          }
        }
      }
    
    }
    img{
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
  .bottom-footer{
    display: flex;
    align-items: center;
    background-color: #303030;
    height: 100px;
    .container{
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .btn{
      background-color: #303030;
      &:hover{
        background-color: $primary-color;
      }
    }
    span{
      font-weight: bold;
      color: $primary-color;
      padding-right: 15px;
     
    }
    i{
      color: #303030;
      background-color: #797979;
      padding: 5px 8px;
      border-radius: 50%;
      margin-right: 10px;
      &:hover{
        background-color: white;
        cursor: pointer;
      }
    }
  }
}
</style>