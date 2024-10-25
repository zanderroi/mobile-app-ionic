<template>
  <ion-app>
    <ion-split-pane content-id="main-content">
      <ion-menu content-id="main-content" type="push">
        <ion-content>
          <Menu />

        </ion-content>
      </ion-menu>
      <ion-router-outlet id="main-content"></ion-router-outlet>

      <ion-header>
        <ion-toolbar>
        <h3>Loyalty Points</h3>
          <ion-buttons slot="start">
            <ion-button @click="toggleMenu">
              <svg viewBox="0 0 180 60" width="60" height="50">
                <rect rx="15" ry="15" width="100" height="20" fill="#d71921"></rect>
                <circle cx="95" cy="7.5" r="20" fill="#e6b849"></circle>
                <rect y="40" rx="15" ry="15" width="100" height="20" fill="#d71921"></rect>
              </svg>
            </ion-button>
          </ion-buttons>
        </ion-toolbar>
      </ion-header>
    </ion-split-pane>
  </ion-app>
</template>

<script setup lang="ts">
import {
  IonApp,
  IonContent,
  IonIcon,
  IonItem,
  IonLabel,
  IonList,
  IonListHeader,
  IonMenu,
  IonMenuToggle,
  IonNote,
  IonRouterOutlet,
  IonSplitPane,
  IonHeader,
  IonToolbar,
  IonButtons,
  IonButton,
} from '@ionic/vue';
import { ref } from 'vue';
import Menu from './components/Menu.vue';


// Function to toggle the menu
const toggleMenu = () => {
  const menu = document.querySelector('ion-menu');
  menu.open(); // You can also use `menu.toggle();` if you want to toggle the menu state.
};
</script>

<style scoped>
/* Add your existing styles here */
</style>