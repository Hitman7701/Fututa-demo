<script setup>
import Header from './components/Header.vue'
import FrontPage from './components/FrontPage.vue'
import ArticleCard from './components/ArticleCard.vue'
import Footer from './components/Footer.vue'

import data from './assets/data/articles.json'
</script>

<template>
  <div>
    <Header />
    <main>
      <FrontPage :frontPage="data.frontPage" />
      <div class="cards">
        <ArticleCard v-for="article in data.articlesList" :key="article.id" :article="article" />
      </div>
    </main>
    <Footer />
  </div>
</template>

<style scoped>
.cards {
  /* border: blue 1px solid; */
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  justify-content: space-around;
  margin-top: 100px;
  padding: 0 30px;
}
</style>
<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather:wght@300;400;700&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap');
</style>
