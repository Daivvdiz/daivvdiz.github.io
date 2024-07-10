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
            projectNames: ['Project 1', 'Project 2'],
            routeProfile: [],
          },
          {
            title: 'Development',
            projectNames: ['Project ', 'Project 2'],
            routeProfile: [],
          },
          {
            title: 'Automatization',
            projectNames: ['Project 1', 'Project 2'],
            routeProfile: [],
          },
          {
            title: 'Personal',
            projectNames: ['Project 1', 'Project 2'],
            routeProfile: [],
          },

        ]
      }
    }
  };
</script>

<style scoped>
.topicCardsContainer {
  display: flex;
  width: 100%;
  height: auto;
  justify-content: space-between;
  margin: 5vh 0;
}
</style>