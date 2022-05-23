<template>
  <div class="post">
    <button>張貼動態</button>
    <div class="active">
      <ul>
        <li>
          <img src="@/assets/img/default.png" alt="" />
          <p>邊緣人</p>
        </li>
        <li>
          <img src="@/assets/img/default.png" alt="" />
          <p>追蹤名單</p>
        </li>

        <li>
          <img src="@/assets/img/default.png" alt="" />
          <p>我按讚的貼文</p>
        </li>
      </ul>
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
.post {
  width: 309px;
  border: 2px solid #000;
}
</style>
