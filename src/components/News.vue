<template>
  <div id="news" class="section-news-wrapper">
    <p class="main-title">News</p>
    <carousel :per-page="3" :autoplay="true">
      <slide>
        <NewsCard />
      </slide>
      <slide>
        <NewsCard />
      </slide>
      <slide>
        <NewsCard />
      </slide>
      <slide>
        <NewsCard />
      </slide>
      <slide>
        <NewsCard />
      </slide>
      <slide>
        <NewsCard />
      </slide>
      <slide>
        <NewsCard />
      </slide>
      <slide>
        <NewsCard />
      </slide>
    </carousel>
  </div>
</template>

<script>
const NewsCard = () => import("../components/NewsCard");

export default {
  components: {
    NewsCard,
  },
};
</script>

<style scoped>
.section-news-wrapper {
  display: flex;
  flex-direction: column;
  margin: 0 auto;
  padding: 60px 86px;
  background-color: #af76ff;
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
</style>
