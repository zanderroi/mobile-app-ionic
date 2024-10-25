<template>
  <ion-page>
    <!-- <ion-header :translucent="true">
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-menu-button color="primary"></ion-menu-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-header> -->

    <ion-content :fullscreen="true">
      <ion-grid class="ion-padding">
  
        <ion-row
          class="ion-justify-content-between ion-align-items-center mt-12"
        >
          <ion-col size="auto">
            <div
              class="tier-section flex flex-row justify-center items-center space-x-2"
            >
              <img
                src="/images/crown.png"
                alt="Beginner Tier Icon"
                class="tier-icon w-12 h-12"
              />
              <p class="ion-text-small">Beginner Tier</p>
            </div>
          </ion-col>
          <ion-col size="auto">
            <a href="/" class="view-all"
              >View All <i class="fa-solid fa-chevron-right"></i
            ></a>
          </ion-col>
        </ion-row>

        <ion-row>
          <ion-col size="12">
            <p class="description">
              Earn points by purchasing from our store. Vestibulum ante ipsum
              primis in faucibus orci luctus et.
            </p>
          </ion-col>
        </ion-row>

   
        <ion-row class="ion-justify-content-center ion-align-items-center mt-8">
          <ion-col size="auto">
            <div class="h-36 w-36 bg-red-200 rounded-full flex justify-center items-center">
              <div class="bg-white rounded-full shadow-md h-28 w-28 flex justify-center items-center">0/160</div>
            </div>
          </ion-col>
        </ion-row>

        <ion-row
          class="ion-justify-content-between ion-align-items-center mt-8 mb-4"
        >
          <ion-col size="auto">
            <p class="ion-text-lg">Rewards</p>
          </ion-col>
          <ion-col size="auto">
            <a href="/" class="how-it-works"
              >How it Works <i class="fa-solid fa-chevron-right"></i
            ></a>
          </ion-col>
        </ion-row>

   
        <ion-row
          class="reward-filters ion-align-items-center text-xs flex overflow-x-scroll no-scrollbar flex-nowrap"
        >
          <ion-col size="auto">
            <div class="filter active-filter">All</div>
          </ion-col>
          <ion-col size="auto">
            <div class="filter">Beginner</div>
          </ion-col>
          <ion-col size="auto">
            <div class="filter">Intermediate</div>
          </ion-col>
          <ion-col size="auto">
            <div class="filter">Loyal</div>
          </ion-col>
        </ion-row>

        <ion-row class="reward-item ion-align-items-center mt-4">
          <ion-col size="auto">
            <img
              src="/images/steak.png"
              sizes="(max-width: 600px) 32px, (max-width: 900px) 48px, 64px"
              alt="Steak Fries Veggies"
              class="reward-image"
            />
          </ion-col>
          <ion-col>
            <p class="reward-title">Steak Fries Veggies</p>
            <p class="reward-category">Meat</p>
            <div class="flex flex-row items-center space-x-2">
              <img
                src="/images/crown.png"
                alt="Points Icon"
                class="points-icon"
              />
              <p class="reward-points">20 points</p>
            </div>
          </ion-col>
        </ion-row>
      </ion-grid>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import {
  IonButtons,
  IonContent,
  IonHeader,
  IonMenuButton,
  IonPage,
  IonToolbar,
  IonGrid,
  IonRow,
  IonCol,
} from "@ionic/vue";
</script>

<style scoped>

.view-all,
.how-it-works {
  color: #d71921;
  font-size: 14px;
}

.description {
  color: gray;
  font-size: 12px;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}


.reward-filters {
  gap: 2px;
  padding-bottom: 8px;
  white-space: nowrap;
}

.filter {
  padding: 8px 16px;
  border-radius: 12px;
  background-color: #e0e0e0;
  color: #606060;
  text-align: center;
}

.active-filter {
  background-color: #d71921;
  color: white;
}


.no-scrollbar::-webkit-scrollbar {
  display: none;
}

.no-scrollbar {
  -ms-overflow-style: none; 
  scrollbar-width: none; 
}


.reward-item {
  background-color: #e0e0e0;
  border-radius: 16px;
  padding: 12px;
}

.reward-image {
  height: 48px;
}

.reward-title {
  font-size: 14px;
}

.reward-category {
  font-size: 12px;
  color: #999;
}

.points-icon {
  height: 20px;
}

.reward-points {
  color: #d71921;
  font-size: 12px;
}


/* @media (max-width: 768px) {
  .points-display {
    height: 6rem;
    width: 6rem;
  }
  .points-inner {
    height: 4.5rem;
    width: 4.5rem;
  }
} */
</style>
