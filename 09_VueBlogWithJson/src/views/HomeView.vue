<script setup>
import TheWelcom from "@/components/home/TheWelcom.vue";
</script>

<template>
  <div class="home">
    <header>
        <table class="text-box">
          <td>순번</td>
          <td>제목</td>
          <td>작성자</td>
          <td>조회수</td>
      </table>
    </header>
    <main>
      <TheWelcom />
    </main>
  </div>
</template>

<style scoped>
main {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 70%;
  margin-top: 1.5%;
  margin-left: auto;
  margin-right: auto;
  height: 90vh;
  background-color: rgb(255, 255, 255);
  padding: 13px;
  border: 1px solid black;
  border-radius: 15px;
  width: 90%;
}
.home {
  background-color: rgb(255, 255, 255);
}

.text-box {
  align-items: center;
  
}
td {
  padding: 15px;
  text-align: center;    /* 텍스트를 가운데 정렬합니다 */
}
</style>
