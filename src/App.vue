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
@import url("https://fonts.googleapis.com/css2?family=Chakra+Petch:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700&display=swap");
#app {
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  font-family: "Chakra Petch", sans-serif;
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
