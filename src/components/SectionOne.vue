<template>
  <div class="section-one container-fluid">
    <div class="row">
      <div
        class="
          image
          col-lg-7 col-md-5 col-sm-12
          d-flex
          align-items-center
          justify-content-center
        "
      >
        <img src="@/assets/img/section1.png" alt="" />
      </div>
      <div
        class="
          introduce-content
          col-lg-5 col-md-7 col-sm-12
          d-flex-col
          align-items-center
          justify-content-left
        "
      >
        <div class="item1">GIỚI THIỆU VỀ DPOKER</div>
        <div class="item2">
          Được phát triển bởi đội ngũ những người yêu thích Poker truyền thống,
          DPOKER được tạo ra như là một nền tảng dựa trên công nghệ blockchain
          mang tính cách mạng khi kết hợp yếu tố Phi Tập Trung. DPOKER sẽ cung
          cấp trải nghiệm chơi trò chơi gambling trực tuyến hấp dẫn, sáng tạo và
          an toàn nhất cho tất cả các cộng đồng yêu thích tiền điện tử và poker.
          Mọi chuyện sẽ trở nên dễ dàng khi bạn có thể tham gia Dpoker với đa số
          loại tiền điện tử phổ biến hiện nay. Chúng tôi sẽ tạo ra một nền tảng
          Poker phi tập trung sở hữu đa dạng đối tượng người dùng lớn nhất trên
          thế giới bằng cách xóa bỏ các hạn chế về độ tuổi tham gia, quốc tịch
          người chơi, vấn đề về luật pháp.
        </div>
        <button class="item3">Đăng ký và chơi ngay</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionOne",
  props: {},
};
</script>
<style lang="scss" scoped>
.section-one {
  padding: 40px;
  height: 100vh;
  background-image: url("@/assets/img/background3.PNG");
  background-repeat: no-repeat;
  background-size: cover;
  @media (max-width: 991px) {
    height: 100%;
  }
  .image {
    max-width: 847px;
    width: 100%;
    img {
      width: 100%;
      object-fit: scale-down;
    }
  }
  .introduce-content {
    text-align: left;
    .item1 {
      font-size: 40px;
      color: #ffd601;
      font-weight: 600;
      margin-bottom: 40px;
      @media (max-width: 991px) {
        font-size: 24px;
        margin-bottom: 20px;
      }
      @media (max-width: 661px) {
        font-size: 18px;
        margin: 10px 0;
      }
    }
    .item2 {
      font-size: 16px;
      color: #fff;
      @media (max-width: 991px) {
        font-size: 14px;
      }
      @media (max-width: 661px) {
        font-size: 12px;
      }
    }
    .item3 {
      background-color: #ffd601;
      color: #000;
      font-weight: 600;
      border-radius: 10px;
      height: 40px;
      max-width: 200px;
      margin: 40px 0 20px 0;
      @media (max-width: 991px) {
        height: 30px;
        margin: 20px 0 10px 0;
      }
    }
  }
}
</style>
