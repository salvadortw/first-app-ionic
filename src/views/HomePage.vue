<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Hello</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Bienvenido</ion-title>
        </ion-toolbar>
      </ion-header>

      <div id="container">
        <strong>Ready to create an app?</strong>
        <p>Start with Ionic <a target="_blank" rel="noopener noreferrer"
            href="https://ionicframework.com/docs/components">UI Components</a></p>
        <ion-chip>Default</ion-chip>
        <ion-chip :disabled="true">Disabled</ion-chip>
        <ion-chip :outline="true">Outline</ion-chip>

        <ion-searchbar color="light" class="search-bar" placeholder="Custom Placeholder"></ion-searchbar>
      </div>
    </ion-content>

    <ion-button class="btn">Default</ion-button>
  </ion-page>

</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar, IonButton, IonChip, IonSearchbar } from '@ionic/vue';

</script>

<style scoped>
#container {
  text-align: center;

  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;

  color: #8c8c8c;

  margin: 0;
}

#container a {
  text-decoration: none;
}

.btn {
  width: 200px;
  margin: 0 auto;
  margin-bottom: 5px;
}

.search-bar {
  max-width: 400px;
  margin: 0 auto;
  margin-top: 5px;
  border-radius: 20px;
}

#container ion-searchbar.custom {
  border-radius: 20px ;
}
</style>
