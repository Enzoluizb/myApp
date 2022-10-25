<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Galeria de Fotos</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <div class="conteudo">
        <h1>Nenhuma foto foi adicionada ainda!</h1>
      </div>
      <ion-button color="danger" fill="outline" shape="round" @click="exibirTexto()">
        <ion-icon :icon="add"></ion-icon>
      </ion-button>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
} from "@ionic/vue";
import { add } from "ionicons/icons";


export default defineComponent({
  name: "Tab1Page",
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage },
  setup() {
    const exibirTexto = () => {
      console.log("Teste de onclick")
    }
    return {
      add,
      exibirTexto
    };
  },
  ionViewDidEnter() {
    console.log("Entrou na página");
  },
  ionViewDidLeave() {
    console.log("Saiu da página");
  },
  ionViewWillEnter() {
    console.log("Vai entrar na página");
  },
  ionViewWillLeave() {
    console.log("Vai sair da página");
  },
});
</script>

<style scoped="style">
h1 {
  color: rgb(255, 255, 255);
  background-color: rgb(0, 0, 0);
  font-family: sans-serif;
  font-size: 15px;
  padding: 5px;
  border-radius: 15px;
  margin: 40px 45px;
  box-shadow: 0 0 40px rgb(43, 43, 43);
}
.conteudo {
  text-align: center;
}

</style>
