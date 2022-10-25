<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Mapa do app</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <div class="conteudo">
        <h1>Mapa</h1>
      </div>
      
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';

export default defineComponent({
  name: 'Tab2Page',
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage }
});
</script>

<style>
h1 {
  color: rgb(255, 255, 255);
  background-color: rgb(56, 199, 0);
  font-family: sans-serif;
  font-size: 15px;
  padding: 5px;
  border-radius: 15px;
  margin: 40px 45px;
  box-shadow: 0 0 40px rgb(24, 85, 0);
}
.conteudo {
  text-align: center;
}
</style>