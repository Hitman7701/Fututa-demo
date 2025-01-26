<script setup>
const props = defineProps({
  article: Object,
})
</script>

<template>
  <section>
    <img :src="article.image" alt="" />
    <div>{{ article.category.toUpperCase() }} {{ article.subCategory.toUpperCase() }}</div>
    <div class="title">{{ article.title }}</div>
    <div class="date">{{ article.date }}</div>
  </section>
</template>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  height: 480px;
  width: 280px;
  /* border: red 1px solid; */
  gap: 10px;
  line-height: 20px;
}
section > img {
  height: 65%;
  object-fit: cover;
}

.title {
  font-weight: bold;
}

.date {
  color: #a6a7a7;
}
</style>
