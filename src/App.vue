<script>
  import HeaderComp from "./components/HeaderComp.vue"
  import BodySecondComp from "./components/BodySecondComp.vue"
  import FooterComp from "./components/FooterComp.vue"

  export default{
    name: "App",
    components: {
      HeaderComp,
      BodySecondComp,
      FooterComp
    }
  }
</script>

<template>
  <HeaderComp/>
  <BodySecondComp/>
  <FooterComp/>
</template>

<style>

</style>
