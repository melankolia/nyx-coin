<template>
  <div id="home" class="home">
    <div class="main-wrapper">
      <AppBar />
      <TitleWrapper />
      <MobileVersion />
    </div>
    <SectionTwo />
    <SectionThree />
    <SectionFour />
    <SectionNews />
    <SectionInvestors />
  </div>
</template>

<script>
// @ is an alias to /src
const AppBar = () => import("../components/AppBar");
const TitleWrapper = () => import("../components/TitleWrapper");
const SectionTwo = () => import("../components/SectionTwo");
const SectionThree = () => import("../components/SectionThree");
const SectionFour = () => import("../components/SectionFour");
const SectionNews = () => import("../components/News");
const SectionInvestors = () => import("../components/Investors");
const MobileVersion = () => import("../components/MobileVersion");

export default {
  name: "Home",
  components: {
    AppBar,
    TitleWrapper,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionNews,
    SectionInvestors,
    MobileVersion,
  },
};
</script>

<style scoped>
.main-wrapper {
  background: linear-gradient(1turn, #722dd0, #a036cc);
  background-repeat: no-repeat;
  background-position: center;
  object-fit: cover;
}
</style>
