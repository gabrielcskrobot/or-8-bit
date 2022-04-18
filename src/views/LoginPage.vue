<template>
  <ion-page>  
    <ion-header>
        <ion-toolbar color="primary">
            <ion-buttons slot="start">
                <ion-back-button defaultHref="/"></ion-back-button>
            </ion-buttons>
            <ion-title>Configurações</ion-title>
        </ion-toolbar>
    </ion-header>    
    <ion-content :fullscreen="true">
      <!-- Conteudo aqui -->
      Configurações
    </ion-content>      

  </ion-page>
</template>
<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';


export default  defineComponent({
  name: 'LoginPage',
  components: {IonHeader, IonToolbar, IonTitle, IonContent, IonPage }
});
</script>
