<template>
  <div class="header">
    <div class="container">
      <div class="logo">MetaWall</div>
      <div class="img">
        <div class="img-content" @click="isShow()">
          <img src="../../assets/img/default.png" alt="user" />
          <p>王小明</p>
        </div>
        <div class="menu" v-show="showMenu">
          <ul>
            <li>我的貼文牆</li>
            <li>修改個人資料</li>
            <li>登出</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const showMenu = ref(false);
    const isShow = () => {
      console.log("1");
      showMenu.value = !showMenu.value;
    };
    return { showMenu, isShow };
  },
};
</script>

<style scoped lang="scss">
.header {
  width: 100%;
  border-bottom: 2px solid #000;
  .container {
    width: 1024px;
    margin: 0 auto;
    padding: 15px 5px;
    display: flex;
    align-content: center;
    justify-content: space-between;
    align-items: center;
    .logo {
      font-size: 26px;
      font-weight: bold;
      cursor: pointer;
    }
    .img {
      .img-content {
        display: flex;
        align-items: center;
        position: relative;
      }
      .menu {
        position: absolute;
        top: 55px;
        background-color: #fff;
        ul {
          border: 2px solid;
          li {
            padding: 5px;
            border-bottom: 2px solid;
            cursor: pointer;
          }
        }
      }
      p {
        padding: 0px 20px;
        cursor: pointer;
      }

      img {
        width: 30px;
        height: 30px;
        cursor: pointer;
      }
    }
  }
}

@media screen and (max-width: 768px) {
  .header {
    .container {
      width: 100%;
    }
  }
}
</style>
