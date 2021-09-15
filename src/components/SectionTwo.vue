<template>
  <div id="project" class="section-two-wrapper">
    <p class="main-title">Open to all. No Invitation Required</p>
    <div class="switch-wrapper">
      <div
        @click="() => (isActive = 'open')"
        class="switch-item"
        :class="{ 'switch-item-active': isOpenActive }"
      >
        Open and Transparency
      </div>
      <div
        @click="() => (isActive = 'fun')"
        class="switch-item"
        :class="{ 'switch-item-active': isFunActive }"
      >
        Diversity and Fun
      </div>
    </div>
    <div class="content-wrapper">
      <div v-if="isOpenActive" class="content-item">
        <div class="item">
          <p class="open-font" style="margin-right: 30px">
            Community members, social media influencers and <br />
            artists can join without other agreement attache
          </p>
          <MobileVersion />
        </div>
        <img :src="robotImage" width="420px" height="280px" alt="robot image" />
      </div>
      <div v-else class="content-item">
        <img :src="robotImage" width="420px" height="280px" alt="robot image" />
        <div class="item">
          <p class="open-font" style="margin-left: 30px">
            Community members, social media influencers and <br />
            artists can join without other agreement attache
          </p>
          <MobileVersion />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
const MobileVersion = () => import("../components/MobileVersion");
import robotImage from "../assets/robot.png";

export default {
  components: {
    MobileVersion,
  },
  data() {
    return {
      isActive: "open",
      robotImage,
    };
  },
  computed: {
    isOpenActive() {
      return this.isActive == "open";
    },
    isFunActive() {
      return this.isActive == "fun";
    },
  },
};
</script>

<style scoped>
.section-two-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 auto;
  padding: 60px 86px;
  background-color: #f1e7ff;
}

.main-title {
  font-size: 40px;
  font-weight: 700;
  padding: 0 22px;
  margin: 0px 0px 22px;
  text-align: center;
  line-height: 1.5;
  margin-bottom: 40px;
}

.switch-wrapper {
  display: flex;
  flex-direction: row;
}

.switch-item:hover {
  cursor: pointer;
}

.switch-item {
  font-size: 30px;
  padding: 0px 40px;
  border-radius: 30px;
  margin: 0 30px;
  color: #6b32ba;
  font-weight: normal;
}

.switch-item-active {
  background-color: #e3d1ff;
  font-weight: 700;
}

.content-wrapper {
  margin: 40px 0 0 0;
  justify-content: flex-start;
  align-items: flex-start;
}

.content-item {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: flex-start;
}

.item {
  display: flex;
  flex-direction: column;
}

.open-font {
  text-align: left;
  font-size: 26px;
}
</style>
