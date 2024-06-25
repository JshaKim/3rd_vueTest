<script setup>
import { useRouter } from "vue-router";

const router = useRouter();
const { blog } = defineProps(["blog"]);

function detailView(id) {
  router.push(`/blogs/${id}`);
}
</script>

<template>
  <div class="itemBox">
    <label @click="detailView(blog.id)">{{ blog.title }}</label>
  </div>
</template>

<style scoped>
.itemBox {
  display: flex;
  justify-content: space-between;
  border: 1px solid;
  align-items: center;
  height: 30px;
  margin-bottom: 1%;
}

label {
  margin-left: 1%;
  cursor: pointer;
}

button {
  margin-right: 1%;
}
</style>
