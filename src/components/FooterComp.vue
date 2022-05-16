<template>
  <footer>
    <div class="footer-top">

      <div class="w-70">
        <ul>
          <li>
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <p>DIGITAL COMICS</p>
          </li>
           <li>
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <p>DC MERCHANDISE</p>
          </li>
           <li>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <p>SUBSCRIPTION</p>
          </li>
           <li>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <p>COMIC SHOP LOCATION</p>
          </li>
           <li>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <p>DC POWER VISA</p>
          </li>
        </ul>
      </div>
    </div>
    <div class="footer-mid">
      <div class="w-70">
        <div class="left-col">
          <ul>
            <h2>DC COMICS</h2>
            <li><a href="">Characters</a></li>
            <li><a href="">Comics</a></li>
            <li><a href="">Movies</a></li>
            <li><a href="">Tv</a></li>
            <li><a href="">Games</a></li>
            <li><a href="">Videos</a></li>
            <li><a href="">News</a></li>
          </ul>
            <ul>
            <h2>SHOP</h2>
            <li><a href="">Shop DC</a></li>
            <li><a href="">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="mid-col">
          <ul>
            <h2>DC</h2>
            <li><a href="">Terms Of Use</a></li>
            <li><a href="">Privacy Policy(New)</a></li>
            <li><a href="">Ad Choices</a></li>
            <li><a href="">Advertising</a></li>
            <li><a href="">Jobs</a></li>
            <li><a href="">Subscription</a></li>
            <li><a href="">Talent Workshop</a></li>
            <li><a href="">CPSC Certificates</a></li>
            <li><a href="">Ratings</a></li>
            <li><a href="">Shop Help</a></li>
            <li><a href="">Contact Us</a></li>
          </ul>
        </div>
        <div class="right-col">
          <ul>
            <h2>SITES</h2>
            <li><a href="">DC</a></li>
            <li><a href="">MAD Magazine</a></li>
            <li><a href="">DC Kids</a></li>
            <li><a href="">DC Universe</a></li>
            <li><a href="">DC Power Visa</a></li>
          </ul>
        </div>
        <div class="bg-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="Footer-bg">
        </div>
      </div>
    </div>
    <div class="footer-btm">
      <div class="container w-70">
        <button><a href="#">SIGN-UP NOW!!</a></button>
        <ul>
          <h2>FOLLOW US</h2>
          <li><img src="../assets/img/footer-facebook.png" alt=""></li>
          <li><img src="../assets/img/footer-periscope.png" alt=""></li>
          <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
          <li><img src="../assets/img/footer-twitter.png" alt=""></li>
          <li><img src="../assets/img/footer-youtube.png" alt=""></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name:"FooterComp"

}
</script>

<style lang="scss" scoped>
@import '../assets/style/_vars.scss';
@import '../assets/style/_general.scss';
@import '../assets/style/_utils.scss';


// FOOTER TOP

.footer-top{
  background-color: $project-color;
  display: flex;
  padding: 40px;
  justify-content: space-around;
  ul{
    display: flex;
    list-style: none;
    li{
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin: 10px 30px;
      cursor: pointer;
      img{
        height: 70px;
      }
      p{
        color: white;
        font-size: 13px;
        font-weight: bold;
        padding-left: 10px;
        min-width: max-content;
      }
    }
  }
}
// FOOTER MID
.footer-mid{
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 30px;
  overflow: hidden;
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  ul{
    list-style: none;
    h2{
      color: white;
    }
    li{
      padding-top: 10px;
    }
    a{
      color:#929191;
      text-decoration: none;
      &:hover{
        text-decoration: underline;
      }
      
    }
  }
  .left-col{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    margin-right: 30px;
    ul:last-of-type{
      margin-top: 30px;

    }
  }
  .mid-col{
    display: flex;
    margin-right: 30px;
  }
  .bg-logo{
    display: flex;
    height: 100px;
  }
  img{
    height: 500px;
    padding-left: 350px;
  }
}

// FOOTER BOTTOM
.footer-btm{
  display: flex;
  justify-content: center;
  padding: 50PX;
  background-color: rgb(48, 48, 48);
  button{
    border-style: none;
    border: 2px solid $project-color;
    padding: 20px 25px;
    background-color: rgb(48, 48, 48);
    a{
      font-size: 17px;
      font-weight: bold;
      color: white;
      text-decoration: none;
    }
  }
  ul{
    display: flex;
    list-style: none;
    h2{
      align-self: center;
      color: $project-color;
      margin-right: 30px;
    }
    li{
      padding-right: 30px;
      align-self: center;
      cursor: pointer;
    }
  } 
}



</style>