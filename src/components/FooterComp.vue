<script>
  export default{
      name: "FooterComp",
      data(){
        return{
                
        }
      }
    }
</script>

<template>
  <div id="footer">
    <!-- PARTE LINK FOOTER -->
    <div id="second-bg" class="container d-flex">
      <!-- PRIMA COLONNA -->
      <div>
        <ul>
          <h5>DC COMICS</h5>
          <li>
            <a href="#">Characters</a>
          </li>
          <li>
            <a href="#">Comics</a>
          </li>
          <li>
            <a href="#">Movies</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">Games</a>
          </li>
          <li>
            <a href="#">Videos</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
        </ul>
        
        <ul>
          <h5>SHOP</h5>
          <li>
            <a href="#">Shop DC</a>
          </li>
          <li>
            <a href="#">Shop DC Collectibles</a>
          </li>
        </ul>
      </div>

      <!-- SECONDA COLONNA -->
      <div>
        <ul>
          <h5>DC</h5>
          <li>
            <a href="#">Terms Of Use</a>
          </li>
          <li>
            <a href="#">Privacy policy (New)</a>
          </li>
          <li>
            <a href="#">Ad Choices</a>
          </li>
          <li>
            <a href="#">Advertising</a>
          </li>
          <li>
            <a href="#">Jobs</a>
          </li>
          <li>
            <a href="#">Subscription</a>
          </li>
          <li>
            <a href="#">Talent Workshops</a>
          </li>
          <li>
            <a href="#">CPSC Certificates</a>
          </li>
          <li>
            <a href="#">Ratings</a>
          </li>
          <li>
            <a href="#">Shop Help</a>
          </li>
          <li>
            <a href="#">Contact Us</a>
          </li>
        </ul>
      </div>

      <!-- TERZA COLONNA -->
      <div>
        <ul>
          <h5>SITES</h5>
          <li>
            <a href="#">DC</a>
          </li>
          <li>
            <a href="#">MAD Magazine</a>
          </li>
          <li>
            <a href="#">DC Kids</a>
          </li>
          <li>
            <a href="#">DC Universe</a>
          </li>
          <li>
            <a href="#">DC Powe Visa</a>
          </li>
          <li>
            <a href="#">Videos</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
        </ul>
      </div>

    </div>  

    <!-- PARTE SOCIAL FOOTER -->
    <div id="footer-low">
      <div id="social" class="container d-flex align-items-center justify-content-between">
        <button>SIGN-UP NOW!</button>
        <div class="d-flex">
          <h4>FOLLOW US</h4>
          <img src="/image/footer-facebook.png" alt="">
          <img src="/image/footer-twitter.png" alt="">
          <img src="/image/footer-youtube.png" alt="">
          <img src="/image/footer-pinterest.png" alt="">
          <img src="/image/footer-periscope.png" alt="">
        </div>
      </div>
      
    </div>

  </div>
  
</template>

<style scoped lang="scss">
  #footer{
    background-image: url('/image/footer-bg.jpg');
    
    /* PARTE LINK FOOTER */
    #second-bg{
      background-image: url('/image/dc-logo-bg.png');
      background-repeat: no-repeat;
      background-size: 40%;
      background-position: center right;

      ul{
        margin-bottom: 0.8rem;

        h5{
          color: white;
          margin: 0.6rem 0;
        }

        li{
          list-style-type: none;

          a{
            text-decoration: none;
            color: gray;
            font-size: 0.8rem;
          }        
        }
      }
    } 
    /* PARTE SOCIAL FOOTER */
    #footer-low{
      background-color: rgb(45, 45, 45);

      #social{
        height: 100px;

        button{
          padding: 0.8rem;
          background-color: rgb(45, 45, 45);
          color: white;
          border: 2px solid rgb(0, 136, 245);
        }

        h4{
          color: rgb(0, 136, 245);
          margin: 0 1rem;
        }

        img{
          color: white;
          margin: 0 0.5rem;
        }      
      }    
    }  
    
  }
  
  

  

  

  

  
  

  

  

  
</style>