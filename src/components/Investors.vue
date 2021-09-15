<template>
  <div class="investors-wrapper">
    <p class="main-title">Investors and Partners</p>
    <div class="partner-box">
      <img :src="aelf" alt="aelf" />
      <img :src="alphaCoin" alt="aelf" />
      <img :src="arrington" alt="arrington" />
      <img :src="bac" alt="bac" />
      <img :src="capital" alt="capital" />
      <img :src="ce_yuan" alt="ce_yuan" />
      <img :src="data" alt="data" />
      <img :src="dhvc" alt="dhvc" />
      <img :src="funcity" alt="funcity" />
      <img :src="linkvc" alt="linkvc" />
      <img :src="newsdog" alt="newsdog" />
      <img :src="nodecapital" alt="nodecapital" />
      <img :src="starscapital" alt="stars" />
    </div>
    <p class="main-title">Media</p>
    <div class="media-box">
      <img :src="blockbreeze" alt="blockbreeze" />
      <img :src="coingecko" alt="coingecko" />
      <img :src="coinhills" alt="coinhills" />
      <img :src="forbes" alt="forbes" />
    </div>
    <p class="main-title">Get Connected</p>
    <div class="icon-container">
      <img :src="IconTwitter" height="64px" width="64px" alt="" />
      <img :src="IconTelegram" height="64px" width="64px" alt="" />
      <img :src="IconEmail" height="64px" width="64px" alt="" />
    </div>
  </div>
</template>

<script>
import aelf from "../assets/Investors/aelf.png";
import alphaCoin from "../assets/Investors/alphacoin.png";
import arrington from "../assets/Investors/arrington.png";
import bac from "../assets/Investors/bac.png";
import capital from "../assets/Investors/capital.png";
import ce_yuan from "../assets/Investors/ce_yuan.png";
import data from "../assets/Investors/data.png";
import dhvc from "../assets/Investors/dhvc.png";
import funcity from "../assets/Investors/funcity.png";
import linkvc from "../assets/Investors/linkvc.png";
import newsdog from "../assets/Investors/newsdog.png";
import nodecapital from "../assets/Investors/nodecapital.png";
import starscapital from "../assets/Investors/starscapital.png";
import blockbreeze from "../assets/Media/blockbreeze.png";
import coingecko from "../assets/Media/coingecko.png";
import coinhills from "../assets/Media/coinhills.png";
import forbes from "../assets/Media/forbes.png";
import IconEmail from "../assets/icon-email.svg";
import IconTelegram from "../assets/icon-telegram.svg";
import IconTwitter from "../assets/icon-twitter.svg";

export default {
  data() {
    return {
      aelf,
      alphaCoin,
      arrington,
      bac,
      capital,
      ce_yuan,
      data,
      dhvc,
      funcity,
      linkvc,
      newsdog,
      nodecapital,
      starscapital,
      blockbreeze,
      coingecko,
      coinhills,
      forbes,
      IconTwitter,
      IconEmail,
      IconTelegram,
    };
  },
};
</script>

<style scoped>
.investors-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 auto;
  padding: 60px 86px;
  background: linear-gradient(180deg, #5e17bd, #573084);
}

.main-title {
  font-size: 40px;
  font-weight: 700;
  padding: 0 22px;
  margin: 0px 0px 47px;
  text-align: center;
  line-height: 1.5;
  margin-bottom: 40px;
  color: white;
}

.partner-box {
  margin: 0 0 60px;
  width: 90%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  flex-wrap: wrap;
}

.media-box {
  margin: 0 0 60px;
  width: 90%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  flex-wrap: wrap;
}

.partner-box > img {
  margin: 20px;
}

.media-box > img {
  margin: 20px;
}

.icon-container {
  display: flex;
  flex-direction: row;
  margin: 0 20px;
  justify-content: space-between;
  align-items: center;
}

@media only screen and (max-width: 720px) {
}

.icon-container > img {
  margin: 0 12px;
}
</style>
