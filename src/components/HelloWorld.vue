<template>
  <div class="hello">
    <ion-grid>
      <ion-row class="ion-justify-content-center ion-align-items-center">
        <img alt="Vue logo" src="../assets/logo.png">
        <h1>{{ msg }}</h1>
      </ion-row>
    </ion-grid>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h1 {
  text-align: center;
}
.hello {
  height: 100%;
  display: flex;
  align-items: center;
}
</style>
