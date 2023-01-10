<template>
  <div class="banner-fr">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-7 col-md-6 col-sm-12 wellCome">
          <div class="item1">DPOKER</div>
          <span class="item2" href="">FUN & PSYCHOLOGY TO EARN</span>
          <p class="item3">
            Chào mừng bạn đến với nền tảng Poker phi tập trung kết hợp với công
            nghệ DeFi tốt nhất trên thế giới. Chúng tôi tạo ra nền tảng này với
            mong muốn chiến thắng luôn thuộc về người chơi nhờ vào việc trở
            thành cổng trung gian đảm bảo lợi ích giữa nhà cái và người chơi.
          </p>
          <button class="item4">Đăng ký và chơi ngay</button>
        </div>
        <div
          class="
            col-lg-5 col-md-6 col-sm-12
            d-flex
            align-items-center
            justify-content-center
          "
        >
          <div class="videoTrain">
            <img src="@/assets/img/videoTrain.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyBaner",
  props: {},
};
</script>
<style lang="scss" scoped>
.banner-fr {
  height: 100vh;
  background-image: url("@/assets/img/background2.PNG");
  background-repeat: no-repeat;
  background-size: cover;
  background-image: url("@/assets/img/background1.PNG");
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  @media (max-width: 991px) {
    height: 100%;
  }
  @media (max-width: 662px) {
    padding-bottom: 60px;
  }
}
.container-fluid {
  .wellCome {
    text-align: left;
    margin: 20px 0;
    padding: 40px;
    .item1 {
      color: #ffd601;
      font-size: 60px;
      font-weight: 600;
      @media (max-width: 991px) {
        font-size: 40px;
      }
      @media (max-width: 662px) {
        font-size: 30px;
      }
    }
    .item2 {
      font-size: 20px;
      color: #1a94ff;
      display: block;
    }
    .item3 {
      color: #fff;
      font-size: 16px;
      margin-top: 60px;
      @media (max-width: 991px) {
        margin-top: 20px;
      }
    }
    .item4 {
      background-color: #ffd601;
      height: 40px;
      color: #000;
      font-weight: 600;
      border-radius: 10px;
    }
  }
  .videoTrain {
    text-align: center;
    max-width: 640px;
    width: 100%;
    border: 3px solid rgb(255, 255, 255, 0.2);
    border-radius: 10px;
    img {
      width: 100%;
      object-fit: scale-down;
    }
  }
}
</style>
