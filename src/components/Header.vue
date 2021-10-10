<template>
  <div class="flex-container">
    <h1 class="logoWeb" style="font-size: 45px">Sivevide</h1>
    <div class="router">
      <a href="/" class="link">Trang chủ</a>
      <a href="/about" class="link">Về chúng tôi</a>
    </div>
    <a href="/login" class="linkLogin">Đăng nhập</a>
    <hr
      style="height: 2px; border-width: 0; color: gray; background-color: gray"
    />
  </div>
  <!-- <hr /> -->
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.flex-container {
  display: flex;
  flex-direction: row;
  align-content: center;
  align-items: center;
  /* justify-content: center; */
  justify-content: space-between;
  grid-row-gap: 50px;
  background-color: white;
  overflow: hidden;
}
.router {
  align-content: center;
  align-items: center;
  text-decoration: none;
}
.link {
  padding-right: 50px;
  text-decoration: none;
  color: inherit;
  text-decoration-line: none;
}

.logoWeb {
  color: red;
  margin-left: 100px;
  margin-right: 150px;
}

a {
  font-size: 20px;
  font-weight: 700;
  margin-right: 50px;
}

a:hover {
  color: red;
}

.linkLogin {
  text-decoration: none;
  color: red;
  text-decoration-line: none;
  text-align: right;
  margin-left: auto;
  justify-content: flex-end;
  flex: 1;
  /* margin-right: 0px; */
}
</style>
