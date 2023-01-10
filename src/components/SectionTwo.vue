<template>
  <div id="section2" class="section-two">
    <h2 class="title">CÁC YẾU TỐ NỔI BẬT</h2>
    <div class="container">
      <div class="row">
        <div
          class="item col-lg-4 col-md-6 col-sm-12"
          v-for="(item, idx) in sectionTwoItems"
          :key="item + idx"
          href=""
        >
          <div class="wrap-item">
            <div>
              <img :src="item.img" alt="" />
            </div>
            <div class="tile-style">
              {{ item.title }}
            </div>
            <p class="content-style">{{ item.content }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionTwo",
  props: {},
  data() {
    return {
      sectionTwoItems: [
        {
          id: 1,
          img: require("@/assets/img/section2Img1.png"),
          title: "KIẾM TIỀN THẬT",
          content:
            "Với cơ chế Play-To-Earn, bạn có thể thoải mái kiếm tiền bằng cách thi đấu trực tuyến với những người chơi trên toàn thế giới.",
        },
        {
          id: 2,
          img: require("@/assets/img/section2Img2.png"),
          title: "NFT AVATAR",
          content:
            "Tăng thêm thu nhập với hình đại diện của chính bạn. Tăng cường nhận diện thương hiệu cá nhân",
        },
        {
          id: 3,
          img: require("@/assets/img/section2Img3.png"),
          title: "VIDEO CALL",
          content:
            "Tạo cơ hội cho các người chơi tương tác trực tiếp với nhau Xóa bỏ khoảng cách người chơi trong thế giới Metaverse ",
        },
        {
          id: 4,
          img: require("@/assets/img/section2Img4.png"),
          title: "METAVERSE",
          content:
            "Gặp gỡ bạn bè cũng như đối mặt với các đối thủ trong thế giới ảo 3D.",
        },
        {
          id: 5,
          img: require("@/assets/img/section2Img5.png"),
          title: "PRIVATE NETWORK",
          content:
            "Trở thành người xây dựng mạng lưới riêng và mời người chơi tham gia các trò chơi độc quyền của bạn.",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.section-two {
  min-height: 458px;
  background-image: url("@/assets/img/background2.PNG");
  background-repeat: no-repeat;
  background-size: cover;
  padding: 30px 0;
  .title {
    color: #ffd601;
    font-size: 40px;
    padding: 40px 0 40px 40px;
    text-align: left;
    font-weight: 600;
    @media (max-width: 991px) {
      font-size: 26px;
      padding: 20px 0 10px 40px;
    }
    @media (max-width: 662px) {
      font-size: 24px;
    }
  }
  .item {
    margin: 10px 0;
    .wrap-item {
      min-height: 458px;
      border-radius: 20px;
      border-width: 2px;
      border-style: solid;
      border-color: rgb(245, 241, 241);
      overflow: hidden;
      .tile-style {
        color: #ffd601;
        font-size: 20px;
        font-weight: 600px;
        margin: 15px 0;
      }
      .content-style {
        color: #fff;
        font-size: 14px;
      }
    }
    img {
      max-width: 100%;
      max-height: 100%;
    }
  }
}
</style>
