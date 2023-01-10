<template>
  <div class="header">
    <div class="img-fra">
      <img src="@/assets/img/logo1.png" />
    </div>
    <div class="header-item">
      <a
        v-for="(item, idx) in headerItems"
        :key="item + idx"
        :href="item.href"
        >{{ item.title }}</a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "MyBaner",
  props: {},
  data() {
    return {
      headerItems: [
        {
          id: 1,
          title: "Trang chủ",
          href: "#",
        },
        {
          id: 2,
          title: "Các yếu tố nổi bật",
          href: "#section2",
        },
        {
          id: 3,
          title: "Tại sao phải tham gia Docker Defi",
          href: "#section3",
        },
        {
          id: 4,
          title: "Roadmap",
          href: "#section4",
        },
        {
          id: 5,
          title: "FAQs",
          href: "#section5",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1440px;
  width: 100%;
  height: 97px;
  color: aliceblue;
  padding: 10px 15px 0;
  background: rgba(3, 1, 33, 0.8);
  .header-item {
    display: flex;
    width: 80%;
    justify-content: space-between;
    a {
      @media (max-width: 767px) {
        font-size: 10px;
      }
    }
  }
  .b-text {
    font-weight: 600;
    color: #ffd601;
  }
  a {
    color: #fff;
  }
  .img-fra {
    width: 134px;
    height: 87px;
    left: 61px;
    top: 10px;
    img {
      width: 100%;
      object-fit: scale-down;
    }
  }
}
</style>
