<template>
  <div class="container">
    <h1 class="name">Sidevide</h1>
    <div class="info">
      <h2 style="margin-bottom: 40px">Bài tập môn Dự án</h2>
      <h3>Truờng Đại học Công Nghệ - Đại học Quốc Gia Hà Nội</h3>
    </div>
  </div>
</template>
<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: row;
  align-content: center;
  align-items: center;
  row-gap: 100;
  background-color: white;
  position: absolute;
  gap: 100px;
  margin-left: 200px;
  height: 200px;
}
.info {
  text-align: left;
  margin-left: 100px;
}
.name {
  color: red;
  font-weight: 1000;
}
</style>
