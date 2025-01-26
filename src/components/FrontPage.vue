<script setup>
const props = defineProps({
  frontPage: Object,
})
</script>

<template>
  <section class="front-page">
    <div class="front-image">
      <img :src="frontPage.image" alt="Titan" />
    </div>
    <div>
      <div class="infos">
        <div class="info-absolute">
          <span
            >{{ frontPage.category.toUpperCase() }} {{ frontPage.subCategory.toUpperCase() }}</span
          >
        </div>
        <h1 class="info-absolute">
          <span>{{ frontPage.title }}</span>
        </h1>
      </div>
      <div class="teaser">{{ frontPage.teaser }}</div>
    </div>
  </section>
</template>

<style scoped>
.front-page {
  height: 550px;
  width: 100%;
  /* border: 2px aqua solid; */
  position: relative;
}

.front-image {
  /* border: 2px solid yellow; */
  width: 100%;
  height: 100%;
  position: relative;
  z-index: 1;
}

img {
  height: 100%;
  width: 100%;
  object-fit: cover;
  object-position: bottom;
}

.infos {
  position: absolute;
  z-index: 2;
  left: 150px;
  top: 75px;
  border-left: 5px solid #6325ff;
}

span {
  /* border: 1px yellow solid; */
  color: white;
  background-color: black;
}

h1 {
  font-size: 40px;
  width: 65%;
  line-height: 45px;
}

.teaser {
  position: absolute;
  z-index: 2;
  left: 150px;
  top: 250px;
  width: 60%;
  padding: 20px;
  color: white;
  background: rgb(0 0 0 / 50%);
}
</style>
