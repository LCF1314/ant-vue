<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
    <div id="app">
      <img src="../assets/logo.png">
      <a-button type="primary">Button</a-button>
    </div>
  </div>
</template>

<script lang="ts">
import { Button } from 'ant-design-vue';

import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

@Component({
  components: {
    HelloWorld,
    'a-button': Button
  },
})
export default class Home extends Vue {}
</script>
<style lang="scss">
  
</style>