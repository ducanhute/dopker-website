<template>
  <div class="section-six">
    <div class="container-fluid">
      <div class="title">MEDIA SHOUTOUTS</div>
      <div class="item1">
        <VueSlickCarousel v-bind="settings">
          <div class="mr-10">
            <img src="@/assets/img/section-six1.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six4.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six2.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six5.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six3.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six6.svg" alt="" />
          </div>
        </VueSlickCarousel>
      </div>

      <div class="title">ĐỘI NGŨ ĐỒNG HÀNH</div>
      <div class="item1">
        <VueSlickCarousel v-bind="settings2">
          <div class="mr-10">
            <img src="@/assets/img/section-six7.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six8.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six9.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six10.svg" alt="" />
          </div>
        </VueSlickCarousel>
      </div>

      <div class="title">ĐỐI TÁC CỦA DPOKER</div>
      <div class="item1">
        <VueSlickCarousel v-bind="settings2">
          <div class="mr-10">
            <img src="@/assets/img/section-six7.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six8.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six9.svg" alt="" />
          </div>
          <div class="mr-10">
            <img src="@/assets/img/section-six10.svg" alt="" />
          </div>
        </VueSlickCarousel>
      </div>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";
export default {
  data() {
    return {
      settings: {
        arrows: false,
        dots: true,
        infinite: true,
        slidesToShow: 1,
        slidesToScroll: 1,
        autoplay: true,
        speed: 20000,
        rows: 2,
        autoplaySpeed: 2000,
        cssEase: "linear",
      },
      settings2: {
        arrows: false,
        dots: true,
        infinite: true,
        slidesToShow: 2,
        slidesToScroll: 1,
        autoplay: true,
        speed: 10000,
        autoplaySpeed: 1000,
        cssEase: "linear",
      },
    };
  },
  components: {
    VueSlickCarousel,
  },
};
</script>
<style lang="scss" scoped>
.section-six {
  width: 100%;
  background-image: url("@/assets/img/background4.PNG");
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;
  .container-fluid {
    padding: 20px 0;
  }
  .title {
    padding: 30px;
    color: #ffd601;
    font-size: 30px;
    font-weight: 600;
    margin: 40px 0 40px 0;
    display: flex;
    align-items: center;
    justify-content: center;
    @media (max-width: 662px) {
      margin: 0;
      font-size: 24px;
    }
  }
  .item1 {
    background: rgba(250, 250, 250, 0.1);
  }
  .item1 > div {
    text-align: -webkit-center;
    height: 100%;
  }
  .mr-10 {
    margin: 20px 0 0 0;
  }
}
</style>
