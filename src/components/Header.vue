<script>
  export default{
      name: "Header",
      data(){
        return{
          menuLinks: [
            {
              name: 'CHARACTERS',
              url: '/characters',
              active: false
            },
            {
              name: 'COMICS',
              url: '/comics',
              active: false
            },
            {
              name: 'MOVIES',
              url: '/movies',
              active: false
            },
            {
              name: 'TV',
              url: '/tv',
              active: false
            },
            {
              name: 'GAMES',
              url: '/games',
              active: false
            },
            {
              name: 'COLLECTIBLES',
              url: '/collectibles',
              active: false
            },
            {
              name: 'VIDEOS',
              url: '/videos',
              active: false
            },
            {
              name: 'FANS',
              url: '/fans',
              active: false
            },
            {
              name: 'NEWS',
              url: '/news',
              active: false
            },
            {
              name: 'SHOP',
              url: '/shop',
              active: false
            }
          ]      
        }
      }
    }
</script>

<template>
  <div>
    <div id="header" class="container d-flex align-items-center justify-content-between">
      <div>
        <img src="../assets/image/dc-logo.png" alt="">
      </div>
      <div>
        <ul class="d-flex">
          <li v-for="(elem, index) in menuLinks" :key="index">
            <a href="elem.url">{{ elem.name }}</a>
          </li>
        </ul>
      </div>
    </div>  
  </div>
  
</template>

<style scoped>
  
  #header{
    height: 100px;
  }
  
  img{
    height: 80px;
  }

  a{
    text-decoration: none;
    color: black;
    font-size: 0.8rem;
  }

  li{
    list-style-type: none;
    margin-left: 0.8rem;
    height: 100%;
  }
</style>