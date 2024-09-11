<template>
  <aside class="sidebar">
    <div class="sidebar-header">
      <i class="fas fa-desktop"></i>
      <h2 class="heading-1">
        Información
        <span class="heading-2">
           Académica
        </span>
      </h2>

      <i class="fas fa-times close-icon"></i>
    </div>
    <hr/>
    <ul>
      <li class="item-flex" v-for="item in menuItems" :key="item.id">
        <i class="fas fa-bars"></i>
        <span>{{ item.title }}</span>
      </li>
    </ul>
    <hr/>
    <button class="logout-btn ">
      <i class="fas fa-power-off"></i>
      Cerrar sesión
    </button>
  </aside>
</template>

<script setup>
import { ref } from 'vue'

const menuItems = ref([
  { id: 1, title: 'Item 1' },
  { id: 2, title: 'Item 2' },
  { id: 3, title: 'Item 3' },
  { id: 4, title: 'Item 4' },
  { id: 5, title: 'Item 5' },
  { id: 6, title: 'Item 6' },
  { id: 7, title: 'Item 7' },
])
</script>

<style scoped>


.close-icon{
  position: absolute;
  top:0;
  right:10px;
}

hr {
  width: calc(100% + 20px);
  margin-left: -20px;
  border: none;
  border-top: 1px solid #555;
  margin-top: 10px;
  margin-bottom: 10px;
}

.item-flex {
  display: flex;
  flex-direction: row;
  margin-left: 20px;
  gap: 15px;
}

.sidebar {
  position: fixed;
  top: 0;
  left: 0;
  width: 200px;
  height: 100vh;
  background-color: #333;
  color: white;
  padding: 20px 0;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
}

.sidebar-header, .sidebar ul, .logout-btn {
  position: relative;
  padding-left: 20px;
  padding-right: 20px;
}

.sidebar-header {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}

.sidebar-header h2 {
  margin: 0 10px;
  flex-grow: 1;
  font-size: 16px;
}

.close-icon {
  cursor: pointer;
}

.sidebar ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  flex-grow: 1;
}

.sidebar li {
  display: flex;
  align-items: center;
  padding: 10px 0;
  cursor: pointer;
}

.sidebar li i {
  margin-right: 10px;
}

.logout-btn {
  background: none;
  border: none;
  color: white;
  cursor: pointer;
  display: flex;
  align-items: center;
  padding: 10px 20px;
  font-size: 16px;
  gap: 10px;
}

.logout-btn i {
  margin-right: 10px;
}

.fas {
  width: 20px;
  text-align: center;
}

.heading-1{
  color: gray;
}

.heading-2{
  color: white;
  font-size: 20px;

}


</style>