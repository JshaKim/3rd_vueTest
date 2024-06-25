<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div class="home-button">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <!-- <RouterLink to="/about">About</RouterLink> -->
        <RouterLink to="/post">글 작성하기</RouterLink>
      </nav>
      <h2>게시판</h2>
    </div>
  </header>
  <RouterView />
</template>

<style scoped>
nav {
  display: flex;
  flex-direction: column;
  align-items: center;
}

a {
  margin-left: 10px;
  font-size: 20px;
}
</style>
