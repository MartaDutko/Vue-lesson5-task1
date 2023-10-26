<template >
  <div class="wrapper">
    <favorite-card v-for="card in cardsList" :key="card.id" :card-data="card" />
  </div>
</template>

<script>
import FavoriteCard from "./FavoriteCard.vue";
export default {
  components: { FavoriteCard },
  props: {
    cardsList: {
        type: Array,
        default: ()=>[]
    },
  },
};
</script>

<style lang="css" scoped>
.wrapper{
    width: 50%;
    display: flex;
    justify-content:center;
    background-color: rgb(25, 24, 24);
}
</style>