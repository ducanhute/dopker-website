<template>
  <div id="section4" class="container-fluid">
    <div class="row">
      <div
        class="
          title
          col-lg-4 col-md-4
          d-flex
          align-items-center
          justify-content-center
        "
      >
        ROAD MAP
      </div>
      <div
        class="
          logo
          col-lg-2 col-md-8
          d-none d-lg-flex
          align-items-center
          justify-content-center
        "
      >
        <img src="@/assets/img/section4Logo.png" alt="" />
      </div>
      <div
        class="
          content
          col-lg-5 col-md-12 col-sm-12
          d-flex
          align-items-center
          justify-content-center
        "
      >
        <div class="wrap-item">
          <div class="item1 d-md-flex d-sm-flex">
            <div
              class="
                img
                d-lg-none d-md-flex d-sm-flex
                align-items-center
                justify-content-center
              "
            >
              01
            </div>
            <div>
              <div class="first">Quý 3, 2022</div>
              <div class="text">
                Cho ra mắt MVP (Mininum Viable Product) nội bộ
              </div>
              <div class="text">
                Ra mắt phiên bản thử nghiệm quy mô 1000 người chơi
              </div>
            </div>
          </div>
          <div class="item2 d-md-flex d-sm-flex">
            <div
              class="
                img
                d-lg-none d-md-flex d-sm-flex
                align-items-center
                justify-content-center
              "
            >
              02
            </div>
            <div>
              <div class="first">Quý 4, 2022</div>
              <div class="text">Kêu gọi quỹ đầu tư</div>
              <div class="text">
                Ra mắt phiên bản MVP Public và hạn chế số lượng người tham gia
                trải nghiệm
              </div>
              <div class="text">
                Hoàn tất quy trình chỉnh sửa lỗi từ phiên bản MVP Public
              </div>
            </div>
          </div>
          <div class="item3 d-md-flex d-sm-flex">
            <div
              class="
                img
                d-lg-none d-md-flex d-sm-flex
                align-items-center
                justify-content-center
              "
            >
              03
            </div>
            <div>
              <div class="first">Quý 1, 2023</div>
              <div class="text">
                Ra mắt phiên bản website chính thức của DPoker
              </div>
              <div class="text">
                Ra mắt ứng dụng di động cho 2 hệ điều hành Iphone/Android
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionFour",
  props: {},
};
</script>
<style lang="scss" scoped>
.container-fluid {
  // max-height: 100vh;
  background-image: url("@/assets/img/background1.PNG");
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  @media (max-width: 991px) {
    padding: 10px 0 30px 0;
  }
  @media (max-width: 662px) {
    padding: 0px 30px;
  }
  .text {
    color: #fff;
    font-size: 16px;
    @media (max-width: 662px) {
      font-size: 12px;
    }
  }
  .title {
    color: #ffd601;
    font-size: 40px;
    font-weight: 600;
    @media (max-width: 991px) {
      font-size: 30px;
      font-weight: 550;
      margin: 20px;
    }
    @media (max-width: 662px) {
      font-size: 30px;
      font-weight: 550;
      margin: 20px;
    }
  }
  .logo {
    max-height: 664px;
    margin: 40px 0;
    img {
      max-height: 100%;
      max-width: 100%;
    }
  }
  .content {
    .first {
      color: #ffd601;
      font-size: 22px;
      font-weight: 600;
      @media (max-width: 662px) {
        font-size: 18px;
      }
    }
  }
  .wrap-item {
    .img {
      margin-right: 20px;
      border-radius: 100%;
      background-color: rgb(9, 196, 196);
      color: black;
      width: 50px;
      height: 50px;
      @media (max-width: 662px) {
        display: flex;
        justify-content: center;
        align-items: center;
      }
    }
    text-align: left;
    .item1 {
      margin-bottom: 120px;
      margin-left: -50px;
    }
    .item2 {
      margin-bottom: 120px;
    }
    .item3 {
      margin-left: -50px;
    }
    @media (max-width: 991px) {
      .item1 {
        margin-bottom: 10px;
        margin-left: 0;
      }
      .item2 {
        margin-bottom: 10px;
      }
      .item3 {
        margin-bottom: 10px;
        margin-left: 0;
      }
    }
    @media (max-width: 662px) {
      .item1 {
        margin-bottom: 10px;
        margin-left: 0;
      }
      .item2 {
        margin-bottom: 10px;
      }
      .item3 {
        margin-bottom: 10px;
        margin-left: 0;
      }
    }
  }
}
</style>
