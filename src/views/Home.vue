<template>
  <div class="ion-page">
    <ion-header>
      <ion-toolbar color="primary">
        <ion-buttons slot="start">
          <ion-back-button></ion-back-button>
        </ion-buttons>
        <ion-title color="light">Home</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content padding>
      <HelloWorld msg="Welcome to Your Vue.js + Ionic 4 App!"/>
    </ion-content>
    <ion-footer>
      <ion-toolbar class="ion-text-center" color="primary">
        <ion-button fill="clear" color="light" @click="seeAbout">
          About
          <ion-icon slot="end" name="logo-ionic"></ion-icon>
        </ion-button>
      </ion-toolbar>
    </ion-footer>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

@Component({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {
  seeAbout() {
    this.$router.push('/about');
  }
}
</script>