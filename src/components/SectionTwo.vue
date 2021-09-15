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
        <img class="robot-image" :src="robotImage" alt="robot image" />
      </div>
      <div v-else class="content-item">
        <img class="robot-image" :src="robotImage" alt="robot image" />
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

.main-title {
  font-size: 40px;
  font-weight: 700;
  padding: 0 22px;
  margin: 0px 0px 22px;
  text-align: center;
  line-height: 1.5;
  margin-bottom: 40px;
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

.robot-image {
  max-width: 420px;
  max-height: 280px;
}

@media only screen and (max-width: 500px) {
  .robot-image {
    width: 100%;
  }
}

@media only screen and (max-width: 980px) {
  .switch-item {
    font-size: 20px;
    padding: 20px;
  }

  .content-item {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .open-font {
    text-align: center !important;
    margin: 0 !important;
  }
}
</style>
