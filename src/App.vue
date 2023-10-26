<template>
  <favorite-card-list :cards-list="favoriteSources"/>
</template>

<script>
import FavoriteCardList from "./components/FavoriteCardList.vue";
import { favoriteSources } from "./constans/1_data_google_favorite";

export default {
  name: "App",
  components: {
    FavoriteCardList,
  },
  data() {
    return {
      favoriteSources,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
