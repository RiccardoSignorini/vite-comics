<script>
  export default{
      name: "HeaderComp",
      data(){
        return{
          menuLinks: [
            {
              name: 'CHARACTERS',
              url: '/',
              active: false
            },
            {
              name: 'COMICS',
              url: '/',
              active: true
            },
            {
              name: 'MOVIES',
              url: '/',
              active: false
            },
            {
              name: 'TV',
              url: '/',
              active: false
            },
            {
              name: 'GAMES',
              url: '/',
              active: false
            },
            {
              name: 'COLLECTIBLES',
              url: '/',
              active: false
            },
            {
              name: 'VIDEOS',
              url: '/',
              active: false
            },
            {
              name: 'FANS',
              url: '/',
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
        <img src="/image/dc-logo.png" alt="">
      </div>
      <div>
        <ul class="d-flex">
          <li v-for="(elem, index) in menuLinks" :key="index" :class="elem.active ? 'selected' : ''">
            <a href="elem.url">{{ elem.name }}</a>
          </li>
        </ul>
      </div>
    </div>  
  </div>
  
</template>

<style scoped lang="scss">  
  #header{
    height: 100px;

    img{
      height: 80px;
    } 

    li{
    list-style-type: none;
    margin-left: 0.8rem;
    line-height: 100px;

    a{
      text-decoration: none;
      color: black;
      font-size: 0.8rem;

      &:hover{
        color: rgb(0, 136, 245);
      }    
    }  
    }
    
    .selected{
      border-bottom: 5px solid rgb(0, 136, 245);

      a{
        color: rgb(0, 136, 245);
      }    
    }   
  } 
</style>