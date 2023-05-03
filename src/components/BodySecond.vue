<script>
  export default{
      name: "BodySecond",
      data(){
        return{
          solutions: [
            {
              name: 'DIGITAL COMICS',
              url: '../assets/image/buy-comics-digital-comics.png',
            },
            {
              name: 'DC MERCHANDISE',
              url: '../assets/image/buy-comics-merchandise.png',
            },
            {
              name: 'SUBSCRIPTION',
              url: '../assets/image/buy-comics-subscriptions.png',
            },
            {
              name: 'COMIC SHOP LOCATOR',
              url: '../assets/image/buy-comics-shop-locator.png',
            },
            {
              name: 'DC POWER VISA',
              url: '../assets/image/buy-dc-power-visa.svg',
            }
          ]      
        }
      }
    }
</script>

<template>
  <div id="BodySecond">
      <div class="container">
        <div class="d-flex justify-content-between">
            <div v-for="(elem,index) in solutions" :key="index">
                <div id="alt">
                    <img src="../assets/image/buy-comics-merchandise.png" alt="">
                    <span>{{ elem.name }}</span>
                </div>
            </div>
        </div>
      </div>
  </div>
</template>

<style scoped>
  #BodySecond{
    height: 100px;
    background-color: rgb(0, 136, 245);
    color: white;
  }

  #alt{
    height: 100px;
    align-items: center;
  }

  img{
    height: 50px;
  }
</style>