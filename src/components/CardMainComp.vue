<script>
    export default{
        name: "CardMainComp",
        props: ["card"]
    }
</script>

<template>
    <div class="">
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
        width: 180px;
        height: 250px;
    }
    .cards{
        width: 180px;
        margin: 0 0.5rem;
    }
</style>