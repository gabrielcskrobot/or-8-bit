<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color="primary">
        <ion-buttons slot="start">
          <ion-menu-button></ion-menu-button>
        </ion-buttons>         
        <ion-title>Menssagens</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Menssagens</ion-title>
        </ion-toolbar>
      </ion-header>
          <ion-list-header> Conversas Recentes</ion-list-header>
      
        <ion-item>
          <ion-avatar slot="start">
             <img src="../assets/avatar-finn.png" />
          </ion-avatar>
          <ion-label>
            <h2>Finn</h2>
            <h3>I'm a big deal</h3>
            <p>Listen, I've had a pretty messed up day...</p>
          </ion-label>
        </ion-item>

         <ion-item>
          <ion-avatar slot="start">
            <img src="../assets/avatar-han.png" />
          </ion-avatar>
          <ion-label>
            <h2>Han</h2>
            <h3>Look, kid...</h3>
            <p>I've got enough on my plate as it i...</p>
          </ion-label>
        </ion-item>

         <ion-item>
          <ion-avatar slot="start">
             <img src="../assets/avatar-luke.png" />
          </ion-avatar>
          <ion-label>
            <h2>Luke</h2>
            <h3>Your thoughts betray you</h3>
            <p>I feel the good in you, the conflict...</p>
          </ion-label>
        </ion-item>

         <ion-item>
          <ion-avatar slot="start">
             <img src="../assets/avatar-yoda.png" />
          </ion-avatar>
          <ion-label>
            <h2>Yoda</h2>
            <h3>Size matters not</h3>
            <p>Do or do not. There is no try...</p>
          </ion-label>
        </ion-item>


      
      
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonLabel} from '@ionic/vue';


export default defineComponent({
  name: 'Tab3Page',
  components: {IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonLabel,}
});
</script>
