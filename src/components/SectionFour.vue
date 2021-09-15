<template>
  <div class="section-four-wrapper">
    <div class="wrapper">
      <img
        width="240px"
        height="480px"
        :src="wireframePhone"
        alt="section four"
        class="image-phone"
      />
      <div style="max-width: 65%">
        <p class="main-title">Keep Up with the Latest Trend</p>
        <p class="subtitle">
          Audio Chatroom to connect with the word; Amazing NFTs and virtual
          gifts to share the joy and fun; Grab & Open for mysterious suprise
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import wireframePhone from "../assets/wireframe-phone.png";
export default {
  data() {
    return {
      wireframePhone,
    };
  },
};
</script>

<style scoped>
.section-four-wrapper {
  display: flex;
  flex-direction: column;
  margin: 0 auto;
  padding: 60px 86px;
  background-color: #f1e7ff;
}

.wrapper {
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-top: 20px;
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

.subtitle {
  text-align: left;
  font-size: 26px;
  margin: 20% 0;
}

.image-phone {
  margin-right: 70px;
}

@media only screen and (max-width: 720px) {
  .wrapper {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .image-phone {
    margin: 0;
  }

  .main-title {
    margin-top: 20px;
  }

  .subtitle {
    text-align: center;
  }
}

@media only screen and (max-width: 400px) {
  .section-four-wrapper {
    padding: 30px 30px;
  }
  .main-title {
    font-size: 30px;
    padding: 0;
  }

  .subtitle {
    font-size: 22px;
  }
}
</style>
