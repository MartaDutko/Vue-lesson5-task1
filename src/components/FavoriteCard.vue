<template>
    <div>
        <div class="wrapper">
            <div class="block__img">
                <img :src="cardData.imgSrc" class="img">
            </div>
            <div class="block__tittle">
                <a :href="cardData.link" class="tittle">{{cardData.title}}</a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'FavoriteCard',
        props: {
            cardData: {
                type: Object,
                default: ()=>({})
            },
        },
    }
</script>

<style lang="css" scoped>
.wrapper{
    margin:10px;
}
.block__img{
    padding: 15px;
    border-radius: 50%;
    background-color: rgba(43, 43, 43, 0.432);
}
.img{
    width: 100%;
    height: 30px;
    border-radius: 5px;
}
.block__tittle{
    text-align: center;
}
.tittle{
    text-decoration: none;
    color: white;
    font-size: 20px;
}
</style>