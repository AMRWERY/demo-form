<template>
  <ion-item>
    <ion-label position="fixed">Image</ion-label>
    <br>
    <input type="file" accept="image/*" />
</ion-item>
<ion-button type="submit" expand="block">Submit</ion-button>
</template>

<script lang="ts">
  import { IonItem, IonLabel, IonButton } from '@ionic/vue';

  export default {
    components: { IonItem, IonLabel, IonButton },
  };
</script>