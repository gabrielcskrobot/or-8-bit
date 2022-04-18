<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color="primary">
        <ion-buttons slot="start">
          <ion-menu-button></ion-menu-button>
        </ion-buttons>         
        <ion-title>Campeonatos</ion-title>
        
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        
        <ion-toolbar>
          <ion-title size="large">Campeonatos</ion-title>
         
        </ion-toolbar>
      </ion-header>
      
        <ion-card>
             <img src="../assets/csgo.jpg" />
    <ion-card-header>
      <ion-card-subtitle>Campeonato Counter Strike</ion-card-subtitle>
      <ion-card-title>Campeonato Counter Strike</ion-card-title>
    </ion-card-header>

    <ion-card-content>
      Campeonato Counter Strike
    </ion-card-content>
  </ion-card>

            <ion-card>
               <img src="../assets/lol.jpg" />
    <ion-card-header>
      <ion-card-subtitle>Campeonato Lolzinho</ion-card-subtitle>
      <ion-card-title>Campeonato Lolzinho</ion-card-title>
    </ion-card-header>

    <ion-card-content>
      Campeonato Lolzinho
    </ion-card-content>
  </ion-card>

            <ion-card>
               <img src="../assets/Rocket.jpg" />
    <ion-card-header>
      <ion-card-subtitle>Campeonato Rocket League</ion-card-subtitle>
      <ion-card-title>Campeonato Rocket League</ion-card-title>
    </ion-card-header>

    <ion-card-content>
      Campeonato Rocket League
    </ion-card-content>
  </ion-card>

            <ion-card>
              <img src="../assets/valorant.jpg" />
    <ion-card-header>
      <ion-card-subtitle>Campeonato Valorant</ion-card-subtitle>
      <ion-card-title>Campeonato Valorant</ion-card-title>
    </ion-card-header>

    <ion-card-content>
      Campeonato Valorant
    </ion-card-content>
  </ion-card>

            <ion-card>
               <img src="../assets/frifas.jpg" />
    <ion-card-header>
      <ion-card-subtitle>Campeonato Frifas</ion-card-subtitle>
      <ion-card-title>Campeonato Frifas</ion-card-title>
    </ion-card-header>

    <ion-card-content>
      Campeonato Frifas
    </ion-card-content>
  </ion-card>
      
      
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';


export default defineComponent({
  name: 'Tab2Page',
  components: {IonHeader, IonToolbar, IonTitle, IonContent, IonPage }
});
</script>
