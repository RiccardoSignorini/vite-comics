<script>
  export default{
      name: "MainComp",
      components: {
        CardMainComp
      },
      data(){
        return{
          solutions: [
            {
              name: 'DIGITAL COMICS',
              url: '/image/buy-comics-digital-comics.png',
            },
            {
              name: 'DC MERCHANDISE',
              url: '/image/buy-comics-merchandise.png',
            },
            {
              name: 'SUBSCRIPTION',
              url: '/image/buy-comics-subscriptions.png',
            },
            {
              name: 'COMIC SHOP LOCATOR',
              url: '/image/buy-comics-shop-locator.png',
            },
            {
              name: 'DC POWER VISA',
              url: '/image/buy-dc-power-visa.svg',
            }
          ],
          covers: [
            {
                "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                "price": "$19.99",
                "series": "Action Comics",
                "type": "comic book"
            },
            {
                "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                "price": "$3.99",
                "series": "American Vampire 1976",
                "type": "comic book"
            },
            {
                "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                "price": "$16.99",
                "series": "Aquaman",
                "type": "graphic novel"
            },
            {
                "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                "price": "$2.99",
                "series": "Batgirl",
                "type": "comic book"
            },
            {
                "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                "price": "$3.99",
                "series": "Batman",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                "price": "$2.99",
                "series": "Batman Beyond",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                "price": "$3.99",
                "series": "Batman/Superman",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                "price": "$4.99",
                "series": "Batman/Superman Annual",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                "price": "$5.99",
                "series": "Batman: The Joker War Zone",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                "price": "$6.99",
                "series": "Batman: Three Jokers",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                "price": "$4.99",
                "series": "Batman: White Knight Presents: Harley Quinn",
                "type": "comic book"
            },
            {
                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                "price": "$16.99",
                "series": "Catwoman",
                "type": "graphic novel"
            }
          ]      
        }
      }
    }

    import CardMainComp from "./CardMainComp.vue"
</script>
 
<template>
  <div id="jumbotron" class="position-relative">
    <!-- background image -->
    <span class="px-3 py-2 position-absolute">
      CURRENT SERIES
    </span>
  </div>

  <!-- PROPS SINGOLA CARD CICLATA -->
  <div id="bg-black">
    <div class="d-flex flex-wrap container text-center justify-content-around p-5">
      <CardMainComp v-for="(elem,index) in covers" :key="index" :card="elem"/>
      <button class="px-5 py-2 my-4">
        LOAD MORE
      </button>
    </div>  
  </div>
  
  
  <div id="body-second">
    <div class="container">
      <div class="d-flex justify-content-around">
          <div v-for="(elem,index) in solutions" :key="index" class="d-flex align-items-center">
              <div id="center" class="d-flex align-items-center">
                  <img :src="elem.url" alt="">
                  <span>{{ elem.name }}</span>
              </div>
          </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
  #jumbotron{
    height: 400px;
    background-image: url(/image/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    span{
      color: white;
      background-color: rgb(0, 136, 245);
      bottom: -20px;
    }
    
  }


  #bg-black{
    background-color: rgb(28, 28, 28);
    button{
      background-color: rgb(0, 136, 245);
      // padding: 0 40px;
      color: white;
      border: 0;
    }
  }

  #body-second{
    height: 100px;
    background-color: rgb(0, 136, 245);
    color: white;

    #center{
      line-height: 100px;

      img{
        height: 50px;
        margin: 0 0.8rem;
      }    
    }
  }
  
</style>