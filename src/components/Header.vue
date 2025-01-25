<script setup></script>

<template>
  <section class="header">
    <div><img src="../assets/img/logo-futura-dark.svg" alt="logo futura" /></div>
    <nav>
      <p>SCIENCES <font-awesome-icon :icon="['fas', 'chevron-down']" /></p>
      <p>SANTE <font-awesome-icon :icon="['fas', 'chevron-down']" /></p>
      <p>TECH <font-awesome-icon :icon="['fas', 'chevron-down']" /></p>
      <p>MAISON <font-awesome-icon :icon="['fas', 'chevron-down']" /></p>
      <p>PLANETE <font-awesome-icon :icon="['fas', 'chevron-down']" /></p>
    </nav>
    <div><button>JE M'ABONNE</button></div>
  </section>
</template>

<style scoped>
.header {
  border: 2px solid green;
  height: 60px;
  background: linear-gradient(0.25turn, #be80ff, #6325ff);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 30px;
  font-family:;
}

nav {
  display: flex;
  color: white;
  gap: 30px;
}

nav svg {
  cursor: pointer;
}

button {
  background-color: #ffae14;
  padding: 10px;
  color: white;
  border: none;
  cursor: pointer;
}

button:hover {
  background-color: #d58972;
  font-family:;
}
</style>
