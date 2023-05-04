<script>
  export default{
      name: "BodySecondComp",
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
          ]      
        }
      }
    }
</script>

<template>
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

<style scoped>
  #body-second{
    height: 100px;
    background-color: rgb(0, 136, 245);
    color: white;
  }

  #center{
    line-height: 100px;
  }

  img{
    height: 50px;
  }
</style>