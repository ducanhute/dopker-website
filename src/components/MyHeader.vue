<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info">
      <b-navbar-brand href="#"
        ><img src="@/assets/img/logo1.png"
      /></b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item
            class="text"
            v-for="(item, idx) in headerItems"
            :key="item + idx"
            :href="item.href"
            >{{ item.title }}</b-nav-item
          >
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>

  <!-- <div class="img-fra">
      <img src="@/assets/img/logo1.png" />
    </div>
    <div class="header-item">
      <a
        v-for="(item, idx) in headerItems"
        :key="item + idx"
        :href="item.href"
        >{{ item.title }}</a
      >
    </div> -->
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
.navbar-dark .navbar-nav .nav-link {
  color: rgb(247, 240, 240);
  font-weight: 600;
  font-size: 20px;
  @media (max-width: 341px) {
    font-size: 16 px;
  }
}
.navbar-toggler {
  @media (max-width: 991px) {
    font-size: 2.5rem;
  }
  @media (max-width: 341px) {
    font-size: 1.5rem;
  }
}
ul.navbar-nav {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
}
.bg-info {
  background-color: #030121 !important;
}
</style>
