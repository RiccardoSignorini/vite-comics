<script>
    export default{
        name: "CardMainComp",
        props: ["card"]
    }
</script>

<template>
    <div class="col-lg-2 text-center">
        <img :src="card.thumb" alt="">
        <div class="icon">
            <h6>{{ card.series }}</h6>
            <p>Type: {{ card.type }}</p>
            <p>Price: {{ card.price }}</p>
        </div>
    </div>
</template>

<style scoped lang="scss">
    img{
        width: 11.25rem;
        height: 15.625rem;
    }
    .icon{
        width: 13.25rem;
        color: white;
    }
</style>