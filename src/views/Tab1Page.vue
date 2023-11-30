<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1</ion-title>
        </ion-toolbar>
      </ion-header>

      <!-- Works with params in camelCase 👍 -->
      <!-- <IonNav :root="NavSubComponent" :rootParams="message"/> -->

      <!-- Doesn't work with kebab-case while it should 💥 -->
      <IonNav :root="NavSubComponent" :root-params="message"/>

    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonNav } from '@ionic/vue';

import NavSubComponent from './NavSubComponent.vue'

const message = {
  msg: 'Hello!'
}
</script>
