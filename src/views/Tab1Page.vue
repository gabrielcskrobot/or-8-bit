<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color='primary'>
        <ion-buttons slot="start">
          <ion-menu-button></ion-menu-button>
        </ion-buttons>         
        <ion-title>Equipes</ion-title>


      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
       
        <ion-toolbar>
          <ion-title size="large">Equipes</ion-title>
        </ion-toolbar>
      </ion-header>
     <ion-fab vertical="bottom" horizontal="end" slot="fixed">
      <ion-fab-button @click="setOpen(true)">
        <ion-icon :icon="add"></ion-icon>
      </ion-fab-button>
    </ion-fab>
      
  
         <ion-list-header> Minhas Equipes</ion-list-header>
      
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
       <ion-list-header> Ranking Mundial</ion-list-header>
        <ion-item>
          <ion-avatar slot="start">
            <img src="../assets/avatar-han.png" />
          </ion-avatar>
          <ion-label>
            <h2>x</h2>
            <h3>Look, kid...</h3>
            <p>I've got enough on my plate as it i...</p>
          </ion-label>
        </ion-item>
    </ion-content>
<ion-modal
  :swipe-to-close="true"
  :is-open="isOpenRef"
  :presenting-element="$parent.$refs.ionRouterOutlet" 
  trigger="trigger-button">
    <ion-page>   
    <ion-header>
        <ion-toolbar color="primary">
            <ion-buttons slot="start">
                <ion-button @click="setOpen(false)">Voltar</ion-button>
            </ion-buttons>
            <ion-title>Configurações</ion-title>
        </ion-toolbar>
    </ion-header>    
    <ion-content :fullscreen="true">
      <!-- Conteudo aqui -->
      Configurações
    </ion-content>      
 
  </ion-page>

</ion-modal>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent, ref  } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonIcon, IonModal , IonFabButton, IonButtons,  } from '@ionic/vue';
import { add} from 'ionicons/icons';

export default  defineComponent({
  name: 'Tab1Page',
  components: {IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonIcon, IonModal , IonFabButton, IonButtons,  },

  setup() {
    const isOpenRef = ref(false);
    const setOpen = (state: boolean) => {
      isOpenRef.value = state;
      console.log('fechando');
    };
    return {
      isOpenRef, 
      setOpen,
      add,
     }
    }
});
</script>
