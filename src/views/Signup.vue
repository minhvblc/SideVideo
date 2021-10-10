<template>
  <div class="bigContainer">
    <div class="container">
      <div class="login-form">
        <form action="" method="post">
          <h1>Đăng ký</h1>
          <div class="input-box">
            <i></i>
            <input
              type="text"
              placeholder="Nhập email"
              v-model="email"
              required
            />
          </div>
          <div class="input-box">
            <i></i>
            <input
              type="password"
              placeholder="Nhập mật khẩu"
              v-model="password"
              required
            />
          </div>
          <div class="input-box">
            <i></i>
            <input
              type="password"
              placeholder="Nhập lại mật khẩu"
              v-model="passwordAgain"
              required
            />
          </div>
          <div class="btn-box">
            <button type="submit">Đăng ký</button>
          </div>
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
      passwordAgain: "",
    };
  },
  methods: {
    register() {
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
  margin-right: 70px;
  width: 70%;
  max-width: 1200px;
  margin-left: auto;
  height: 900px;
}

.login-form {
  width: 60%;
  margin: 20px auto;
  background-color: #ffffff;
  padding: 15px;
  border: 3px dotted #cccccc;
  border-radius: 10px;
  text-align: left;
  box-shadow: 1px 0.5px 0.5px 0.5px #888888;
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
  padding: 7.5px 20px;
  width: 100%;
  border: 1px solid #cccccc;
  outline: none;
  height: 50px;
  border-radius: 10px;
  color: #cccccc;
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

.bigContainer {
  background-image: url("../assets/video.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
