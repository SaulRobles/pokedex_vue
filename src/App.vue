<script setup>
  import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <nav class="nav">
        <RouterLink class="navButtons" to="/"><el-button class="elementButton" type="info">Home</el-button></RouterLink>
        <RouterLink class="navButtons" to="/list"><el-button class="elementButton" type="info">List</el-button></RouterLink>
        <img class="main_logo" src="./assets/backgrounds/logo_principal.png" alt="" />
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>
  .main_logo {
    position: absolute;
    width: 10rem;
    top: 10px;
    right: 15px;
  }
  .nav{
    background: cornflowerblue;
    display: flex;
    justify-content: center;
  }
  .navButtons {
    color: white;
    margin: 1rem;
  }
  .elementButton {
    width: 10rem;
  }
</style>
