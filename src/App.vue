<template>
  <div class="app">
    <!-- Sidebar -->
    <Sidebar />
    <router-view />
  </div>
</template>

<script setup>
import Sidebar from './components/Sidebar.vue'
</script>

<style lang="scss">
:root {
  --primary-color: #4ade80;
  --secondary-color: #64748b;
  --dark: #1e293b;
  --quaternary-color: #334155;
  --light-color: #f5f5f5;
  --sidebar-width: 300px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira Sans', 'sans-serif';
}

body{
  background: var(--light-color);
}

button{
  cursor: pointer;
  appearance: none;
  border: none;
  outline: none;
  background: none;
}

.app{
  display: flex;

  main {
    flex: 1 1 0;
    padding: 2rem;

    @media (max-width: 768px){
      padding-left: 6rem;
    }
  }
}

</style>
