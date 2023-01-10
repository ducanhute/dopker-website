<template>
  <div class="footer container-fluid">
    <div class="wrap-footer row">
      <div class="col-lg-6 col-md-12">
        <div class="footerLogo">
          <img class="logo" src="@/assets/img/logo1.png" />
        </div>
        <div class="wrap-content col-md-12">
          <div
            class="content"
            v-for="(item, index) in mainTitle"
            :key="item + index"
          >
            <span class="content1">
              {{ item.content }}
            </span>
            <span v-if="item.content2" class="content2">
              {{ item.content2 }}
            </span>
          </div>
          <div class="evaluation">
            <div>DPOKER:</div>
            <p>
              Dự án không được thiết kế với mục đích đánh bạc.Thay vào đó, nó
              tập trung vào tinh thần thể thao bằng cách chỉ cung cấp các giải
              đấu poker, sit & go và các trò chơi cạnh tranh tương tự.
            </p>
          </div>
        </div>
      </div>
      <div class="contact col-md-12 col-lg-6">
        <div class="item1">LIÊN HỆ</div>
        <div class="item2">
          <div>Họ và Tên:</div>
          <div>Email:</div>
          <div>Câu Hỏi:</div>
        </div>
        <div class="btn">
          <button class="btn-item">Gửi</button>
        </div>
        <div class="item3">
          <div>CẬP NHẬT THÔNG TIN TẠI ĐÂY:</div>
          <div class="icon">
            <img class="icon1" src="@/assets/img/youtube.svg" alt="" />
            <img class="icon2" src="@/assets/img/tele.svg" alt="" />
            <img class="icon3" src="@/assets/img/face.svg" alt="" />
            <img class="icon4" src="@/assets/img/twitter.svg" alt="" />
            <img class="icon5" src="@/assets/img/discord.svg" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyFooter",
  props: {},
  data() {
    return {
      mainTitle: [
        {
          id: 1,
          content: "TRANG CHỦ",
          content2: "Whitepaper",
        },
        {
          id: 2,
          content: "CÁC YẾU TỐ NỔI BẬT",
          content2: "Điều khoản dịch vụ",
        },
        {
          id: 3,
          content: "TẠI SAO NÊN THAM GIA DROPER",
          content2: "Chính sách dự án",
        },
        {
          id: 4,
          content: "ROADMAP",
          content2: "Trách nhiệm người chơi",
        },
        {
          id: 5,
          content: "FAQS",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.footer {
  background-image: url("@/assets/img/background1.PNG");
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 100vh;
  width: 100%;
  .wrap-footer {
    position: relative;
    display: flex;
    height: 100%;
    .footerLogo {
      position: absolute;
      top: 0;
      left: 0;
    }
    .wrap-content {
      margin-top: 20vh;
      padding-left: 20px;
      flex: 1;
      @media (max-width: 991px) {
        margin-top: 12vh;
      }

      @media (max-width: 662px) {
        margin-top: 14vh;
      }

      .content {
        display: flex;
        margin: 10px 0;
        .content1 {
          width: 60%;
          text-align: left;
          color: #fff;
          @media (max-width: 991px) {
            font-size: 20px;
          }
          @media (max-width: 661px) {
            font-size: 12px;
          }
        }
        .content2 {
          --height: 30px;
          line-height: var(--height);
          min-height: var(--height);
          border-radius: 5px;
          padding: 0 5px;
          text-align: left;
          font-weight: 600;
          color: #000;
          background-color: #00a3ff;
          @media (max-width: 991px) {
            font-size: 20px;
          }
          @media (max-width: 661px) {
            font-size: 11px;
            --height: 12px;
            line-height: var(--height);
            min-height: var(--height);
          }
        }
      }
      .evaluation {
        padding: 200px 30px 0 0;
        @media (max-width: 991px) {
          padding: 20px 30px 0 0;
          font-size: 24px;
        }
        @media (max-width: 662px) {
          padding: 20px 30px 0 0;
        }
        div {
          color: #ffd601;
          font-weight: 600;
          text-align: left;
        }
        p {
          color: #fff;
          font-size: 16px;
          @media (max-width: 991px) {
            font-size: 20px;
            text-align: left;
          }
          @media (max-width: 662px) {
            font-size: 12px;
            text-align: left;
          }
        }
      }
    }
    .contact {
      flex: 1;
      padding: 20px;
      .item1 {
        margin-top: 10%;
        text-align: left;
        color: #fff;
        font-size: 20px;
        @media (max-width: 991px) {
          font-size: 20px;
          margin-top: 10px;
          padding-left: 20px;
        }
      }
      .item3 > div:first-of-type {
        color: #fff;
        font-size: 20px;
        text-align: left;
      }
      .item3 {
        padding-top: 60px;
        .icon > img {
          margin: 10px 20px;
          width: 30px;
          height: 30px;
        }
        .icon {
          text-align: left;
        }
      }

      .item2 {
        margin-top: 30px;
        padding: 20px 10px;
        text-align: left;
        width: 80%;
        color: #000;
        background-color: #ececec;
        @media (max-width: 991px) {
          width: 100%;
          margin-top: 10px;
          padding: 20px 20px;
          font-size: 20px;
        }
      }
      .item2 > div {
        padding: 6px 0;
        font-weight: 500;
      }
      .btn {
        width: 80%;
        margin-right: 20%;
        text-align: right;
        @media (max-width: 991px) {
          margin-right: -24px;
          width: 100%;
        }

        .btn-item {
          min-width: 80px;
          min-height: 40px;
          border-radius: 8px;
          background-color: #ffd601;
          color: #000;
          font-size: 16px;
          @media (max-width: 991px) {
            min-width: 140px;
            min-height: 40px;
            font-size: 24px;
          }
          @media (max-width: 661px) {
            min-width: 80px;
            min-height: 40px;
            font-size: 16 px;
          }
        }
      }
    }
  }
}
</style>
