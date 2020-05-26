<template>
  <div id="app">
    <h1>{{ message }}</h1>
    <img alt="Vue logo" src="./assets/logo.png" /><br>
    数字もできるよ {{ count }}<br>
    <p>このinputを編集すると見出し(message)がリアルタイムに変わる</p>
    <input v-model="message">
    <p>このinputを編集するとカウントが(count)変わる</p>
    <input type="number" v-model="count"><br>
    <!-- v-on:イベント でイベントを起こせる -->
    <button v-on:click="alert">アラートがでるボタン</button>
    <!-- v-on:イベント と @イベント は同じ（省略記法）-->
    <button @click="incrementCounter">(count)が増えるボタン</button>
    <!-- 引数も指定可能 --->
    <button @click="incrementsCounter(5)">(count)が5ずつ増えるボタン</button>
    <button @click="incrementsCounter(count)">(count)が(count)ずつ増えるボタン（2倍になる）</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: "Hello Vue!",
      count: 1
    };
  },
  methods: {
    alert(){
      // 呼び出されるとアラートがでます
      window.alert("ぴこーん！")
    },
    incrementCounter(){
      // スクリプト内でdataを参照するには this. のあとに変数名
      this.count++
    },
    // add だけ増加する
    incrementsCounter(add){
      this.count += add
    }
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
