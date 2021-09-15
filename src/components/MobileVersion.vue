<template>
  <div class="mobile-version">
    <p class="comingsoon-text" style="margin-right: 32px">Coming Soon</p>
    <img
      :src="androidImage"
      style="margin-right: 32px"
      width="42px"
      height="42px"
      alt=""
    />
    <img
      :src="appleImage"
      style="margin-right: 32px"
      width="42px"
      height="42px"
      alt=""
    />
  </div>
</template>

<script>
import androidImage from "../assets/android.png";
import appleImage from "../assets/apple.png";
export default {
  data() {
    return {
      androidImage,
      appleImage,
    };
  },
};
</script>

<style scoped>
.comingsoon-text {
  font-size: 26px;
  color: #999;
}

.mobile-version {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  margin-top: 40px;
}
</style>
