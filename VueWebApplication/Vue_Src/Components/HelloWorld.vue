<template>
  <div class="hello">
    <h1>{{ start + number }}</h1>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import { Component, Prop } from 'vue-property-decorator';

@Component
export default class HelloWorld extends Vue {
  @Prop({ type: Number, default: 99 })
  start: number;

  msg: string = 'ECOS...........';
  number: number = 0;

  mounted() {
    window.setInterval(() => {
      this.number++;
    }, 1000);
  }

  gooto() {
    console.log('gooto');
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
