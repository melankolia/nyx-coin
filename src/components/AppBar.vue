<template>
  <div class="topnav">
    <div>
      <a href="#home">Home</a>
      <a href="#project">Project</a>
      <a href="#application">Application</a>
      <a href="#news">News</a>
    </div>
    <div class="icon-container">
      <img :src="IconTwitter" height="28px" width="28px" alt="" />
      <img :src="IconTelegram" height="28px" width="28px" alt="" />
      <img :src="IconEmail" height="28px" width="28px" alt="" />
    </div>
  </div>
</template>

<script>
import IconEmail from "../assets/icon-email.svg";
import IconTelegram from "../assets/icon-telegram.svg";
import IconTwitter from "../assets/icon-twitter.svg";

export default {
  data() {
    return {
      IconEmail: IconEmail,
      IconTelegram: IconTelegram,
      IconTwitter: IconTwitter,
    };
  },
};
</script>

<style scoped>
.topnav {
  overflow: hidden;
  background-color: #9f36cb;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  position: fixed; /* Set the navbar to fixed position */
  top: 0; /* Position the navbar at the top of the page */
  width: 100%; /* Full width */
  z-index: 11;
}

.topnav a {
  float: left;
  color: #f2f2f2;
  text-align: center;
  margin: 20px 20px;
  text-decoration: none;
  font-size: 19px;
  font-weight: 700;
  line-height: 1.75rem;
  color: hsla(0, 0%, 100%, 0.6);
}

.icon-container {
  display: flex;
  flex-direction: row;
  margin: 0 20px;
  justify-content: space-between;
  align-items: center;
}

.icon-container img {
  margin: 0 4px;
}

a:focus {
  color: #fff;
}
</style>
