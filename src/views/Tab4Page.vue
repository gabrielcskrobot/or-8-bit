<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color='primary'>
        <ion-buttons slot="start">
          <ion-menu-button></ion-menu-button>
        </ion-buttons>        
        <ion-title>Perfil</ion-title>
        <ion-chip slot="secondary" color="tertiary">
        <ion-label> Orbs - 666 </ion-label>
        <ion-icon :icon="close"></ion-icon>
        </ion-chip>
        
        <ion-buttons slot="end">
          <ion-button id="menu-button">
            <ion-icon slot="icon-only" :icon="ellipsisVertical" :ios="ellipsisHorizontal" :md="ellipsisVertical"></ion-icon>
          </ion-button>
        </ion-buttons>        

        <ion-popover trigger="menu-button" side="bottom" alignment="end">
          <ion-content>
            <ion-list>
              <ion-item :button="true" :detail="false">
                <ion-label>Configurações</ion-label>
              </ion-item>
              <ion-item :button="true" :detail="false">
                <ion-label>Sair</ion-label>
              </ion-item>
              <ion-item :button="true" :detail="false">
                <ion-label>Código QR</ion-label>
              </ion-item>
            </ion-list>
          </ion-content>
        </ion-popover>
        
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Perfil</ion-title>
        </ion-toolbar>
      </ion-header>

      <ion-card class="ion-text-center">
              <ion-chip slot="end" color="tertiary">
              <ion-label> 666 </ion-label>
              <ion-icon :icon="close"></ion-icon>
              </ion-chip>
          <img src="../assets/avatar-finn.png" style="border-radius: 50%"/>
          <ion-card-header>
            <ion-card-subtitle>Destination</ion-card-subtitle>
            <ion-card-title>Madison, WI</ion-card-title>
          </ion-card-header>
          <ion-card-content>
            Founded in 1829 on an isthmus between Lake Monona and Lake Mendota, Madison was named the capital of the
            Wisconsin Territory in 1836.
          </ion-card-content>
        </ion-card>
    
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent} from '@ionic/vue';
import {personCircleOutline, ellipsisHorizontal, ellipsisVertical} from 'ionicons/icons';

export default defineComponent({
  name: 'Tab3Page',
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage },

  setup() {
    return {
     personCircleOutline,
     ellipsisHorizontal,
     ellipsisVertical, 
    }
  }
});
</script>
