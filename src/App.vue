<template>
  <div id="app">
    <span class="button-wrap"><a href="#" class="easy-button button button-circle button-caution" @click="play"></a></span>
  </div>
</template>

<script>
let soundUrl = require("file-loader!./easy.mp3");
export default {
  name: 'app',
  methods: {
    play () {
      new Audio(soundUrl).play()
    }
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">
@import "buttons.css";
.easy-button {
  width: 300px;
  height: 300px;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
