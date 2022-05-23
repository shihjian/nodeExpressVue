<template>
  <div class="search">
    <div class="select">
      <select>
        <option>最新文章</option>
      </select>
    </div>
    <div class="searchBar">
      <div class="searchBox">
        <input type="text" placeholder="搜尋貼文" />
        <div class="box">5</div>
      </div>
    </div>
  </div>
</template>

<script>
// import { ref } from "vue";
export default {
  setup() {
    return {};
  },
};
</script>

<style scoped lang="scss">
.search {
  display: flex;
  .select {
    width: 175px;
    border: 2px solid #000;
    select {
      width: 100%;
      padding: 10px 16px;
      font-size: 20px;
      border: none;
    }
  }
  .searchBar {
    width: 100%;
    height: 100%;
    margin-left: 12px;
    border: 2px solid #000;
    .searchBox {
      display: flex;
      input[placeholder] {
        width: 100%;
        font-size: 20px;
      }
      .box {
        width: 46px;
        height: 46px;
        background-color: #03438d;
        border-left: 2px solid #000;
      }
    }
  }
}
</style>
