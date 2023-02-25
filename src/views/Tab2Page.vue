<template>
  <ion-segment v-model="segment" mode="md">
    <ion-segment-button value="1">
      Segment 1
    </ion-segment-button>
    <ion-segment-button value="2">
      Segment 2
    </ion-segment-button>
    <ion-segment-button value="3">
      Segment 3
    </ion-segment-button>
  </ion-segment>

  <ion-card v-show="segment === '1'" class="ion-no-margin ion-padding-bottom">
    <ion-card-header>
      <PageOne />
    </ion-card-header>
  </ion-card>
  <ion-card v-show="segment === '2'" class="ion-no-margin ion-padding-bottom">
    <ion-card-header>
      <PageTwo />
    </ion-card-header>
  </ion-card>
  <ion-card v-show="segment === '3'" class="ion-no-margin ion-padding-bottom">
    <ion-card-header>
      <PageThree />
    </ion-card-header>
  </ion-card>
</template>

<script lang="ts" setup>
import { IonSegment, IonSegmentButton, IonCard, IonCardHeader } from '@ionic/vue';
import PageOne from '@/components/PageOne.vue';
import PageTwo from '@/components/PageTwo.vue';
import PageThree from '../components/PageThree.vue';
import { ref } from 'vue';
const segment = ref('1');
</script>
