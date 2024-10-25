<template>
  <ion-list>
    <div class="p-4">
      <div class="flex flex-row items-center space-x-4">
        <img src="/images/girl.jpg" alt="Description of Image" class="w-14 h-14 rounded-full" />
        <div class="flex flex-row items-center space-x-6">
          <img src="/images/crown.png" alt="Description of Image" class="w-8" />
          <p class="text-xs">0 points </p>
          <i class="fa-solid fa-chevron-right text-xs" style="color: #d71921"></i>
        </div>
      </div>
      <div>
        <p class="text-lg">Chou Tzuyu</p>
        <p class="text-xs text-gray-400">+63 912 345 6789</p>
      </div>
    </div>

    <div class="p-2">
      <ion-item router-link="/" router-direction="root" class="active space-x-2" lines="none" :detail="false">
      <i class="fa-solid fa-house"></i>
      <ion-label class="label-xs">Home</ion-label>
    </ion-item>
    <ion-item router-link="/order-now" router-direction="root" class="inactive space-x-2" lines="none" :detail="false">
      <i class="fa-solid fa-drumstick-bite"></i>
      <ion-label class="label-xs">Order Now!</ion-label>
    </ion-item>
    <ion-item router-link="/notifications" router-direction="root" class="inactive space-x-2" lines="none" :detail="false">
      <i class="fa-solid fa-bell"></i>
      <ion-label class="label-xs">Notifications</ion-label>
      <div class="w-8 h-8 rounded-full bg-yellow-500 flex items-center justify-center">
        <span class="text-xs text-white">4</span>
      </div>
    </ion-item>
    <ion-item router-link="/store" router-direction="root" class="inactive space-x-2" lines="none" :detail="false">
      <i class="fa-solid fa-store"></i>
      <ion-label class="label-xs">Store Locator</ion-label>
    </ion-item>
    <ion-item router-link="/faqs" router-direction="root" class="inactive space-x-2" lines="none" :detail="false">
      <div class="rounded-full w-5 h-5 bg-gray-200 flex justify-center items-center">
        <i class="fa-solid fa-question text-xs"></i>
      </div>
      <ion-label class="label-xs">FAQs</ion-label>
    </ion-item>
    <hr>

    <ion-item router-link="/order-now" router-direction="root" class="inactive space-x-2 mt-2" lines="none" :detail="false">
      <i class="fa-solid fa-bag-shopping"></i>
      <ion-label class="label-xs">My Orders</ion-label>
      <div class="w-8 h-8 rounded-full bg-yellow-500 flex items-center justify-center">
        <span class="text-xs text-white">2</span>
      </div>
    </ion-item>
    <ion-item router-link="/order-now" router-direction="root" class="inactive space-x-2 mt-2" lines="none" :detail="false">
      <i class="fa-solid fa-user"></i>
      <ion-label class="label-xs">My Accounts</ion-label>
    </ion-item>
    <ion-item router-link="/order-now" router-direction="root" class="inactive space-x-2 mt-2" lines="none" :detail="false">
      <i class="fa-solid fa-heart"></i>
      <ion-label class="label-xs">My Favorites</ion-label>
    </ion-item>
    <ion-item router-link="/order-now" router-direction="root" class="inactive space-x-2 mt-2" lines="none" :detail="false">
      <i class="fa-solid fa-location-dot"></i>
      <ion-label class="label-xs">Order Tracker</ion-label>
    </ion-item>
    <ion-item router-link="/order-now" router-direction="root" class="inactive space-x-2 mt-2" lines="none" :detail="false">
      <i class="fa-solid fa-clock-rotate-left"></i>
      <ion-label class="label-xs">Order History</ion-label>
    </ion-item>
    <ion-button size="default" color="danger" class="text-xs px-4 w-60">Logout</ion-button>
    </div>
    

    
  </ion-list>
</template>

<script setup lang="ts">
import { IonList, IonItem, IonLabel, IonButton } from '@ionic/vue';
</script>

<style scoped>
.label-xs {
  font-size: 0.80rem; /* You can adjust the size here as needed */
}

.active {
  color: black;
}

.inactive {
  color: gray;
}


</style>