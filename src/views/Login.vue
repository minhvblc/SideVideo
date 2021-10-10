<template>
  <div class="bigContainer">
    <div class="container">
      <div class="login-form">
        <form action="" method="post">
          <h1>Đăng nhập</h1>
          <div class="input-box">
            <i></i>
            <input
              v-model="email"
              type="text"
              placeholder="Nhập email"
              required
            />
          </div>
          <div class="input-box">
            <i></i>
            <input
              v-model="password"
              type="password"
              placeholder="Nhập mật khẩu"
              required
            />
          </div>
          <div class="btn-box">
            <button type="submit" @click="login">Đăng nhập</button>
          </div>
          <p
            style="
              margin-bottom: 15px;
              font-style: italic;
              text-color: grey;
              font-size: 18px;
            "
          >
            Chưa có tài khoản?
          </p>
          <a href="/signup" class="signup">Đăng ký ngay</a>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Login",
  components: {},
  data() {
    return {
      email: "",
      password: "",
    };
  },
  methods: {
    login() {
      alert("username :" + this.email + " pasword" + this.password);
    },
  },
};
</script>

<style scoped>
* {
  padding: 0px;
  margin: 0px;
  font-family: sans-serif;
  font-size: 20px;
  box-sizing: border-box;
}

.container {
  padding-top: 200px;
  margin-right: 100px;
  width: 70%;
  max-width: 1200px;
  margin-left: auto;
  height: 800px;
}

.bigContainer {
  background-image: url("../assets/video.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

.login-form {
  width: 60%;
  margin: 20px auto;
  background-color: #ffffff;
  padding: 15px;
  border-radius: 10px;
  text-align: left;
  box-shadow: 2px 2px 2px 2px #888888;
}

h1 {
  color: red;
  font-size: 30px;
  margin-bottom: 30px;
  text-align: left;
  margin-top: 20px;
}

.input-box {
  margin-bottom: 30px;
}

.input-box input {
  padding: 7.5px 15px;
  width: 100%;
  border: 1px solid #cccccc;
  outline: none;
  height: 50px;
  font-size: 18px;
}

.btn-box {
  text-align: left;
  margin-top: 30px;
}

.btn-box button {
  padding: 7.5px 15px;
  border-radius: 10px;
  background-color: red;
  color: #ffffff;
  border: none;
  outline: none;
  margin-bottom: 30px;
}

.signup {
  text-align: left;
  color: red;
  font-size: 18px;
}
</style>
