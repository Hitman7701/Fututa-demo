<script setup>
import Header from './components/Header.vue'
import FrontPage from './components/FrontPage.vue'
import ArticleCard from './components/ArticleCard.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div>
    <Header />
    <main>
      <FrontPage />
      <ArticleCard />
    </main>
    <Footer />
  </div>
</template>

<style scoped></style>
<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather:wght@300;400;700&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap');
</style>
