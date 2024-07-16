<script setup>
import ProjectCard from './Card.vue'
</script>

<template>
  <div class="topicCardsContainer">
    <ProjectCard v-for="(card, index) in cards" :key="index" :name="card.title" :contents="card.projectNames" :routeProfile="card.routeProfile" />
  </div>
</template>

<script>
  export default {
    data() {
      return {
        cards: [
          {
            title: 'Data Analytics',
            projectNames: ['Sales Insight', 'Market Trends', 'Customer Segmentation'],
            routeProfile: [],
          },
          {
            title: 'Development',
            projectNames: ['Task Manager', 'Weather App', 'E-commerce Site', 'Portfolio Website'],
            routeProfile: [],
          },
          {
            title: 'Automation',
            projectNames: ['Home Automation', 'Factory Control'],
            routeProfile: [],
          },
          {
            title: 'Personal',
            projectNames: ['Daily Journal', 'Fitness Tracker', 'Travel Blog', 'Recipe Book', 'Budget Planner'],
            routeProfile: [],
          },

        ]
      }
    }
  };
</script>

<style scoped>
@media screen and (min-width: 1024px){
  .topicCardsContainer {
    display: flex;
    width: 100%;
    height: auto;
    justify-content: space-evenly;
    margin: 5vh 0;
  }
}
</style>