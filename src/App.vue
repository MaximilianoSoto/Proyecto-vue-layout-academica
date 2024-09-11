<script setup>
import Header from './components/Header.vue'
import SideBar from "@/components/SideBar.vue";
import Cards from "./components/Cards.vue";
</script>

<template>
  <SideBar></SideBar>
  <div class="main-content">
    <Header></Header>
    <Cards></Cards>


  </div>




</template>

<style scoped>
.main-content{
  margin-left: 200px;





}

</style>
