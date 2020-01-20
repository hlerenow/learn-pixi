<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
  </div>
</template>

<script lang="ts">
// @ is an alias to /src
import {
  Component, Prop, Vue, Watch, Model,
} from 'vue-property-decorator';
import * as PIXI from 'pixi.js';

@Component
export default class Home extends Vue {
  private name:string = 'leo';

  created():void {
    const { name } = this;
    console.log('created', name);
  }
}
</script>
