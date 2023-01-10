<template>
  <div id="app" style="overflow: hidden">
    <MyHeader />
    <MyBaner />
    <SectionOne />
    <SectionTwo />
    <SectionThree />
    <SectionFour />
    <SectionFive />
    <SectionSix />
    <Footer />
    <!-- <HelloWmyIntroduceorld msg="Welcome to Vue.js App" msg2="234" /> -->
  </div>
</template>
<script>
// import HelloWorld from "./components/HelloWorld.vue";
import MyHeader from "./components/MyHeader.vue";
import MyBaner from "./components/MyBanner.vue";
import SectionOne from "./components/SectionOne.vue";
import SectionTwo from "./components/SectionTwo.vue";
import SectionThree from "./components/SectionThree.vue";
import SectionFour from "./components/SectionFour.vue";
import SectionFive from "./components/SectionFive.vue";
import SectionSix from "./components/SectionSix.vue";
import Footer from "./components/MyFooter.vue";
export default {
  name: "App",
  components: {
    MyHeader,
    MyBaner,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    SectionSix,
    Footer,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  // margin-top: 60px;
}
body {
  margin: 0;
}
</style>
