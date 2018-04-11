<template>
  <div id="app">
    <h1>Home Page View</h1>
    <div class="com">
      <p>HIHIHIHI</p>
    </div>
    <router-view/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Component from 'vue-class-component';

@Component
export default class App extends Vue {
  mounted() {
    console.log('hihihi22');
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.com {
  p {
    color: aqua;
  }
}
</style>
