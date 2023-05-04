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
    <!-- PARTE ALTA FOOTER -->
    <div id="second-bg" class="container d-flex">
      <!-- PRIMA COLONNA -->
      <div>
        <ul>
          <h5>DC COMICS</h5>
          <li>Characters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
        </ul>
        
        <ul>
          <h5>SHOP</h5>
          <li>Shop DC</li>
          <li>Shop DC Collectibles</li>
        </ul>
      </div>

      <!-- SECONDA COLONNA -->
      <div>
        <ul>
          <h5>DC</h5>
          <li>Terms Of Use</li>
          <li>Privacy policy (New)</li>
          <li>Ad Choices</li>
          <li>Advertising</li>
          <li>Jobs</li>
          <li>Subscription</li>
          <li>Talent Workshops</li>
          <li>CPSC Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contact Us</li>
        </ul>
      </div>

      <!-- TERZA COLONNA -->
      <div>
        <ul>
          <h5>SITES</h5>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Powe Visa</li>
          <li>Videos</li>
          <li>News</li>
        </ul>
      </div>

    </div>  

  </div>
  
</template>

<style scoped>
  #footer{
    background-image: url('/image/footer-bg.jpg');
  }
  
  #second-bg{
    background-image: url('/image/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-size: 40%;
    background-position: center right;
  }

  h5{
    color: white;
    margin: 0.6rem 0;
  }

  ul{
    margin-bottom: 0.8rem;
  }

  li{
    color: gray;
    list-style-type: none;
    font-size: 0.8rem;
  }
</style>