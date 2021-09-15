<template>
  <div class="title-wrapper">
    <div class="main-title">
      Decentralized Drop-in Chatroom for Crypto World
    </div>
    <div class="desc-title">
      NFTs, Digital Collectables, and virtual gifts.....
    </div>
    <div class="text">
      <span class="txt-whitepaper">WhitePaper</span>
    </div>
    <img class="image-phone" :src="ImagePhone" alt="image phone" />
  </div>
</template>

<script>
import ImagePhone from "../assets/img-phone.png";

export default {
  data() {
    return {
      ImagePhone,
    };
  },
};
</script>

<style scoped>
.title-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.main-title {
  color: white;
  font-size: 44px;
  font-weight: 700;
  padding: 0 22px;
  margin: 120px 0px 22px;
  text-align: center;
  line-height: 1.5;
}

.desc-title {
  color: white;
  line-height: 1.4;
  font-size: 30px;
  margin: 22px 166px 0px;
  margin-bottom: 40px;
}

.text {
  background: #fff;
  padding: 12px 0;
  border-radius: 40px;
  width: 32%;
  box-shadow: 0 0.2rem 0.3rem 0 #7a00cd;
  z-index: 10;
}

.text:hover {
  cursor: pointer;
}

.txt-whitepaper {
  font-size: 28px;
  font-weight: 700;
}

.image-phone {
  width: 80%;
  height: 80%;
  margin-top: -200px;
}
</style>
