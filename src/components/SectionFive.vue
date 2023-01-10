<template>
  <div id="section5" class="container-fluid">
    <div class="row justify-content-center">
      <div class="col-lg-12">
        <h2 class="title">FAQ</h2>
      </div>
      <div
        class="col-lg-10 col-md-10 col-sm-10 phone-style"
        v-for="(item, idx) in content"
        :key="item + idx"
      >
        <div class="wrap">
          <div class="it-1-2">
            <div class="it-1">{{ item.id }}</div>
            <div class="it-2">{{ item.title }}</div>
          </div>
          <button data-toggle="collapse" :data-target="`#${item.name}`">
            <img class="it-3" src="@/assets/img/icon-up.svg" alt="" />
          </button>
        </div>
        <div :id="`${item.name}`" class="collapse jd" style="color: #fff">
          {{ item.jd }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionFour",
  props: {},
  data() {
    return {
      content: [
        {
          id: 1,
          name: "one",
          title: "Dropker là gì?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
        {
          id: 2,
          name: "two",
          title: "Các đồng tiền sẽ được sử dụng để thanh toán?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
        {
          id: 3,
          name: "three",
          title: " Làm sao rút tiền từ hệ thống ra ngoài?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
        {
          id: 4,
          name: "four",
          title: "Các token nào sẽ được sử dụng?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
        {
          id: 5,
          name: "five",
          title: "Tương lai sẽ có token riêng cho DPOKER không?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
        {
          id: 6,
          name: "six",
          title: "Tôi phải sử dụng ví điện tử nào để tham gia DPOKER?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
        {
          id: 7,
          name: "seven",
          title: "Số tiền tối thiểu để rút tiền và gửi tiền là bao nhiêu ?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
        {
          id: 8,
          name: "eight",
          title: "Tôi có thể nhận được 100% số tiền cược của mình ?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
        {
          id: 9,
          name: "night",
          title: "Tôi có thể chơi DPOKER với BNB hay không ?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
        {
          id: 10,
          name: "ten",
          title: "Các đồng tiền sẽ được sử dụng để thanh toán?",
          jd: "DPOKER là một nền tảng nền tảng Poker phi tập trung với sự kết hợp của công nghệ Blockchain và DeFi",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.container-fluid {
  background-image: url("@/assets/img/background2.PNG");
  background-repeat: no-repeat;
  background-size: cover;
  @media (max-width: 662px) {
    .jd {
      font-size: 12px;
    }
  }
  .title {
    color: #ffd601;
    font-size: 50px;
    font-weight: 600px;
    padding-left: 40px;
    margin-top: 30px;
  }
  .wrap {
    width: 100%;
    height: 85px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 20px 0 0 0;
    background-color: #07093e;
    .it-1-2 {
      display: flex;
      align-items: center;
      width: 90%;
      color: white;
    }
    .it-1 {
      width: 59px;
      height: 59px;
      color: white;
      background-color: #00a3ff;
      font-size: 30px;
      border-radius: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 0 10px;
      @media (max-width: 662px) {
        font-size: 24px;
        width: 44px;
        height: 44px;
      }
    }
    .it-2 {
      margin: 0 20px;
      font-weight: 600;
      @media (max-width: 662px) {
        margin: 0;
        font-size: 12px;
      }
    }
    .it-3 {
      width: 30px;
      height: 30px;
      @media (max-width: 662px) {
        width: 20px;
        height: 20px;
      }
    }
    button {
      border: none;
      color: white;
      margin: 0 20px;
    }
  }
}
</style>
