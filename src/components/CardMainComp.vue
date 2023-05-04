<script>
    export default{
        name: "CardMainComp",
        props: ["card"]
    }
</script>

<template>
    <div class="col-2">
        <img :src="card.thumb" alt="">
        <div class="cards text-center">
            <h6>{{ card.series }}</h6>
            <p>Type: {{ card.type }}</p>
            <span>Price: {{ card.price }}</span>
        </div>
    </div>
</template>

<style scoped lang="scss">
    img{
        width: 11.25rem;
        height: 15.625rem;
    }
    .cards{
        width: 11.25rem;
        color: white;
    }
</style>