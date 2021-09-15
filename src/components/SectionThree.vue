<template>
  <div id="application" class="section-three-wrapper">
    <p class="main-title">High Performance & Effiency</p>
    <div class="feature-wrapper">
      <div class="feature-item">
        <img width="201px" :src="imageDecentralized" alt="decentralized" />
        <p>Decentralized</p>
        <span style="font-size: 20px; line-height: 1.5">
          Blockchain-Based protocol to safeguard the network to run smoothly
          without hierarchy
        </span>
      </div>
      <div class="feature-item">
        <img width="201px" :src="imageUnique" alt="unique" />
        <p>Unique and Simple</p>
        <span style="font-size: 20px; line-height: 1.5">
          Customized and user-friendly interface for all participants
        </span>
      </div>
      <div class="feature-item">
        <img width="201px" :src="imageStable" alt="stable" />
        <p>Stable and Trustworthy</p>
        <span style="font-size: 20px; line-height: 1.5">
          Each transaction and exchange are recorded on chain for transparency
        </span>
      </div>
      <div class="feature-item">
        <img width="201px" :src="imageNeutral" alt="neutral" />
        <p>Neutral and Effiency</p>
        <span style="font-size: 20px; line-height: 1.5">
          Combined with the benefits of blockchain to ensure the integrity and
          validity of mechanism
        </span>
      </div>
    </div>
  </div>
</template>

<script>
import imageDecentralized from "../assets/decentralized.png";
import imageUnique from "../assets/unique.png";
import imageStable from "../assets/stable.png";
import imageNeutral from "../assets/neutral.png";

export default {
  data() {
    return {
      imageDecentralized,
      imageUnique,
      imageStable,
      imageNeutral,
    };
  },
};
</script>

<style scoped>
.section-three-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 auto;
  padding: 60px 86px;
}

.main-title {
  font-size: 40px;
  font-weight: 700;
  padding: 0 22px;
  margin: 0px 0px 47px;
  text-align: center;
  line-height: 1.5;
  margin-bottom: 40px;
}

.feature-wrapper {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
}

.feature-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin: 0 14px;
  max-width: 260px;
}

.feature-item > p {
  font-size: 24px;
  font-weight: 700;
}

@media only screen and (max-width: 720px) {
  .feature-wrapper {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
