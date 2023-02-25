<template>
  <ion-list-header lines="full">
    <ion-label>Create Offer</ion-label>
  </ion-list-header>

  <form>
    <ion-item>
      <ion-label position="floating">Tagline</ion-label>
      <ion-input></ion-input>
    </ion-item>

    <ion-item>
      <ion-label position="floating">Offer Type</ion-label>
      <ion-select>
        <ion-select-option value="discount">Discount</ion-select-option>
        <ion-select-option value="buy_one_get_one">Buy One Get One</ion-select-option>
        <ion-select-option value="free_shipping">Free Shipping</ion-select-option>
      </ion-select>
    </ion-item>

    <ion-item>
      <ion-label position="fixed">Valid From</ion-label>
      <ion-input required placeholder="" type="date"></ion-input>
    </ion-item>

    <ion-item>
      <ion-label position="fixed">Valid Till</ion-label>
      <ion-input required placeholder="" type="date"></ion-input>
    </ion-item>
  </form>
  
    <ion-button expand="block">Next</ion-button>
</template>

<script lang="ts">
import { IonListHeader, IonLabel, IonItem, IonSelect, IonSelectOption, IonButton } from '@ionic/vue';

export default {
  components: { IonListHeader, IonLabel, IonItem, IonSelect, IonSelectOption, IonButton },
}
</script>