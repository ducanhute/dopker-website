<template>
  <div id="section3" class="section-three">
    <div class="header">TẠI SAO NÊN THAM GIA DROPKER?</div>
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
  name: "SectionThree",
  props: {},
  data() {
    return {
      sectionTwoItems: [
        {
          id: 1,
          img: require("@/assets/img/section3Img1.svg"),
          title: "Tính phi tập trung",
          content:
            "Với cấu trúc phi tập trung người chơi sẽ hoàn toàn yên tâm được về sự minh bạch với chi phí tốt nhất.",
        },
        {
          id: 2,
          img: require("@/assets/img/section3Img2.svg"),
          title: "NFT AVATAR",
          content:
            " Là công trung gian, Dpoker sẽ đảm bảo lợi nhuận trực tiếp của người chơi, khoản lợi nhuận này sẽ đến từ chi phí giao dịch giữa người chơi và nhà cái.",
        },
        {
          id: 3,
          img: require("@/assets/img/section3Img3.svg"),
          title: "VIDEO CALL",
          content:
            "Với hệ sinh thái rộng lớn và số lượng người chơi mang tính toàn cầu. Chính vì vậy, bạn có thể chơi với bất cứ ai.",
        },
        {
          id: 4,
          img: require("@/assets/img/section3Img4.svg"),
          title: "METAVERSE",
          content:
            "Nhanh chóng tiện lợi hỗ trợ 24/7 với đa dạng cổng giao dịch.Tiết kiệm chi phí, thời gian nhờ vào tốc độ xử lý giao dịch và công nghệ Blockchain ",
        },
        {
          id: 5,
          img: require("@/assets/img/section3Img5.svg"),
          title: "PRIVATE NETWORK",
          content:
            "Hero Book, Dragon Pool và tương lai sẽ có thêm rất nhiều Game Fi NFT được tích hợp vào hệ sinh thái. ",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.section-three {
  background-image: url("@/assets/img/background1.PNG");
  background-repeat: no-repeat;
  background-size: cover;
  padding: 0 0 30px 0;
  .header {
    padding: 100px 0;
    color: #ffd601;
    font-size: 40px;
    font-weight: 600;
    @media (max-width: 991px) {
      font-size: 26px;
      padding: 60px 0 20px 40px;
      text-align: left;
    }
    @media (max-width: 662px) {
      font-size: 24px;
      padding: 60px 0 20px 40px;
    }
  }
  .item {
    margin: 10px 0;
    .wrap-item {
      min-height: 284px;
      border-width: 2px;
      border-style: solid;
      border-color: rgb(245, 241, 241);
      overflow: hidden;
      @media (max-width: 991px) {
        min-height: 260px;
      }
      @media (max-width: 662px) {
        min-height: 200px;
      }
      .tile-style {
        color: #ffd601;
        font-size: 20px;
        font-weight: 600px;
        margin: 15px 0;
        @media (max-width: 991px) {
          margin: 10px 0;
        }
        @media (max-width: 662px) {
          margin: 4px 0;
        }
      }
      .content-style {
        color: #fff;
        font-size: 14px;
        padding: 10px 20px;
        @media (max-width: 991px) {
          padding: 4px 20px;
        }
        @media (max-width: 662px) {
          padding: 4px 20px;
        }
      }
    }
    img {
      max-width: 100%;
      max-height: 100%;
      margin: 14px auto;
    }
  }
}
</style>
