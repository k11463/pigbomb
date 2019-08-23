<template>
  <div class="bg">
    <div class="title">炊挖旅遊</div>
    <div class="searchBox">
      <div class="inputBox">
        <input type="text" placeholder="輸入心儀地點、活動或城市..." />
      </div>
      <div class="searchBtn">
        <div class="btn">
          <i class="fas fa-search"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    console.log("Component mounted.");
  }
};
</script>

<style lang="scss" scoped>
.bg {
  font-family: "標楷體";
  height: 100%;
  .title {
    font-size: 28px;
    font-weight: bold;
    border: 1px solid #000;
    float: left;
    padding: 0 80px 0 80px;
  }
  .searchBox {
    border: 1px solid #000;
    padding: 0 80px 0 80px;
    float: left;
    height: 100%;
    .inputBox {
      float: left;
      input {
        width: 440px;
        height: 32px;
        border: none;
        border-radius: 4px 0 0 4px;
        padding-left: 12px;
        color: #000;
        font-weight: bold;
      }
      input::placeholder {
        font-size: 16px;
        color: #8e8e8e;
        font-weight: 100;
      }
    }
    .searchBtn {
      width: 60px;
      float: left;
      height: 100%;
      display: flex;
      align-items: center;
      .btn {
        width: 100%;
        height: 34px;
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: #26bec9;
        border: 1px solid #277c7c17;
        margin-bottom: 2px;
        border-radius: 0 4px 4px 0;
        cursor: pointer;
        i {
          color: white;
        }
      }
      .btn:hover {
        background-color: #22abb5;
      }
    }
  }
}
</style>
