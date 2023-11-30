<template>
    <IonHeader>
      <IonToolbar>
        <IonTitle>Tab 1</IonTitle>
      </IonToolbar>
    </IonHeader>

    <IonContent class="ion-padding">
        <IonLabel >
            {{ msg }}
        </IonLabel>
    </IonContent>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonLabel, IonTitle, IonToolbar } from '@ionic/vue';

defineProps<{
    msg: string
}>()
</script>