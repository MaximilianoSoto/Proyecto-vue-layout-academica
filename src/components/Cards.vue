<script setup>

</script>

<template>
  <div class="content-grid">
    <div v-for="i in 4" :key="i" class="card small-card"></div>
    <div class="card large-card"></div>
    <div class="card large-card"></div>
    <div class="card medium-card"></div>
    <div class="card medium-card"></div>
    <div class="card medium-card"></div>
    <div class="card medium-card"></div>
    <div class="card medium-card"></div>
    <div class="card medium-card"></div>
  </div>

</template>

<style scoped>

.content-grid {
  display: grid;
  position: relative;
  top: -13rem;
  grid-template-columns: repeat(4, 1fr);
  gap: 15px;
  padding: 20px;
}

.card {
  background-color: gray;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.small-card {
  height: 100px;
}

.medium-card {
  height: 150px;
  grid-column: span 2;
}

.large-card {
  height: 150px;
  grid-column: span 2;
}

</style>