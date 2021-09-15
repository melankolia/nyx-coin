<template>
  <div class="card-wrapper">
    <img width="304px" :src="newsExample" alt="news" />
    <p>Nyx Blockchain Progress Report</p>
  </div>
</template>

<script>
import newsExample from "../assets/news-example.png";

export default {
  data() {
    return {
      newsExample,
    };
  },
};
</script>

<style scoped>
.card-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 6px;
  border-radius: 2%;
  background-color: white;
  margin: 0 50px;
}
</style>
