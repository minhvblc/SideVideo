<template>
  <div class="about">
    <img src="../assets/laptop.jpg" alt="banner" class="banner" />
    <h1 style="margin-top: 200px">Về Sidevide</h1>
    <hr />
    <h2>Đây là bài tập lớn môn Dự án của nhóm</h2>
    <h2>
      Sidevide là một website giúp người dùng dễ dàng tải video chỉ với một cú
      click chuột
    </h2>

    <div class="container">
      <img src="../assets/people.png" alt="people" class="peopleImg" />
      <div>
        <h1>Thành viên</h1>
        <hr />
        <ul style="text-align: left; margin-left: 50px">
          <li>Hoàng Thanh Long</li>
          <li>Vũ Mạnh Hùng</li>
          <li>Nguyễn Đức Minh</li>
          <li>Hiếu</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
.banner {
  height: 300px;
  width: 100%;
  width: 100%;
  height: 550px;
  object-fit: cover;
}

.peopleImg {
  height: 350px;
}

hr {
  background-color: red;
  height: 3px;
  border: 0;
  width: 700px;
  margin-bottom: 50px;
}

.container {
  display: flex;
  flex-direction: row;
  align-content: center;
  align-items: center;
  justify-content: center;
  gap: 100px;
  margin-left: 100px;
  margin-top: 300px;
  margin-bottom: 150px;
  width: 100%;
}

li {
  margin-bottom: 20px;
  font-size: 20px;
  font-weight: bold;
}
</style>
