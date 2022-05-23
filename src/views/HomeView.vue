<template>
  <div class="home">
    <navbar />

    <div class="section">
      <div class="container">
        <search />
      </div>
      <div class="postCard">
        <postCard />
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import navbar from "@/components/homePage/header.vue";
import search from "@/components/homePage/search.vue";
import postCard from "@/components/postCard/postCard.vue";

export default {
  name: "HomeView",
  components: {
    navbar,
    search,
    postCard,
  },
};
</script>
<style scoped lang="scss">
.section {
  max-width: 1024px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  .container {
    width: 100%;
    padding: 15px 5px;
    // display: flex;
    // align-content: center;
    // justify-content: space-between;
    align-items: center;
  }
}

@media screen and (max-width: 768px) {
  .section {
    width: 100%;
    .postCard {
      display: none;
    }
  }
}
</style>
