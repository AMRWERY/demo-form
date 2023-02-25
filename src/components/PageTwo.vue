<template>
    <ion-item>
      <ion-label position="floating">Description</ion-label>
      <ion-textarea></ion-textarea>
  </ion-item> 
  
  <ion-item>
    <ion-label position="floating">Term and Condition</ion-label>
    <ion-textarea></ion-textarea>
  </ion-item>
  
  <ion-button expand="block">Next</ion-button>
</template>

<script lang="ts">
  import { IonItem, IonLabel, IonTextarea, IonButton } from '@ionic/vue';

  export default {
    components: { IonItem, IonLabel, IonTextarea, IonButton },
  };
</script>