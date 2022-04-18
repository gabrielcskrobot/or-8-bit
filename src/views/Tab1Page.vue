<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color='primary'>
        <ion-buttons slot="start">
          <ion-menu-button></ion-menu-button>
        </ion-buttons>         
        <ion-title>Equipes</ion-title>

        <ion-buttons slot="secondary">
          <ion-button color="secondary" id="menu-button">
            <ion-icon slot="icon-only" :icon="ellipsisVertical" :ios="ellipsisHorizontal" :md="ellipsisVertical"></ion-icon>
          </ion-button>
        </ion-buttons>        

        <ion-popover trigger="menu-button" side="bottom" alignment="end">
          <ion-content>
            <ion-list>
              <ion-item :button="true" :detail="false">
                <ion-label>Loja</ion-label>
              </ion-item>
            </ion-list>
          </ion-content>
        </ion-popover>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
       
        <ion-toolbar>
          <ion-title size="large">Equipes</ion-title>
        </ion-toolbar>
      </ion-header>
     <ion-fab vertical="bottom" horizontal="end" slot="fixed">
      <ion-fab-button>
        <ion-icon :icon="add"></ion-icon>
      </ion-fab-button>
    </ion-fab>
      
      <ExploreContainer name="" />
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonIcon,} from '@ionic/vue';
import { add } from 'ionicons/icons';
import ExploreContainer from '@/components/ExploreContainer.vue';

export default  defineComponent({
  name: 'Tab1Page',
  components: { ExploreContainer, IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonIcon,},

  setup() {
    return {
      add,
     }
    }
});
</script>
