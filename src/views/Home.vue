<template>
  <div class="home">
    <img src="../assets/video.jpg" alt="" sizes="" srcset="" class="img" />
    <div class="input">
      <input v-model="url" placeholder="Insert video url" type="url" />
      <button @click="sendUrl">Download</button>
    </div>
    <div style="height: 300px"></div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
  data() {
    return {
      url: "",
    };
  },
  methods: {
    sendUrl() {
      alert(this.url);
    },
  },
};
</script>

<style scoped>
.img {
  width: 100%;
  height: 450px;
  object-fit: cover;
}
.input {
  width: 50%;
  height: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
  top: -50px;
  margin: 0 auto;
  background-color: white;
  border-radius: 5px;
  position: relative;
  box-shadow: 2px 2px 2px 2px #888888;
}
.home {
  align-content: center;
  justify-content: center;
  align-items: center;
}
input {
  width: 70%;
  height: 50px;
  margin-right: 30px;
  border: white;
  font-size: 16px;
}
button {
  background-color: red;
  height: 60px;
  width: 20%;
  border-radius: 5px;
  border: white;
  box-shadow: 1px 1px 1px 1px #888888;
  color: white;
  font-size: 16px;
  font-weight: 700;
}
</style>
