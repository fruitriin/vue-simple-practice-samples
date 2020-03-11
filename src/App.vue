<template>
  <div id="app">
    <h1>{{ message }}</h1>
    <img alt="Vue logo" src="./assets/logo.png" /><br>
    数字もできるよ {{ count }}<br>
    <p>このinputを編集すると見出し(message)がリアルタイムに変わる</p>
    <input v-model="message">
    <p>このinputを編集するとカウントが(count)変わる</p>
    <input type="number" v-model="count">
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: "Hello Vue!",
      count: 1
    };
  }
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
