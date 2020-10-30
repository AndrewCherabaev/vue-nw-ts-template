<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h3>
      Features:
    </h3>
    <ul>
      <li>non-strict typescript</li>
      <li><a href="https://github.com/vuejs/vue-class-component" target="_blank" rel="noopener"> class components </a></li>
      <li><a href="https://github.com/kaorun343/vue-property-decorator" target="_blank" rel="noopener"> property decorators </a></li>
      <li><a href="https://nwjs.io" target="_blank" rel="noopener"> nwjs as dev env </a></li>
      <li>no babel at all</li>
    </ul>
    <h3>Installed CLI Plugins</h3>
    <ul>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-typescript" target="_blank" rel="noopener">typescript</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-vuex" target="_blank" rel="noopener">vuex</a></li>
    </ul>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class HelloWorld extends Vue {
  @Prop() msg: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
