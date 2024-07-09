<script setup>
import TopicCard from './Card.vue'
</script>

<template>
  <div class="topicCardsContainer">
    <TopicCard v-for="(card, index) in cards" :key="index" :title="card.title" :projectNames="card.projectNames"/>
  </div>
</template>

<script>
  export default {
    components: {
      TopicCard
    },
    data() {
      return {
        cards: [
          {
            title: 'Data Analytics',
            projectNames: ['Project 1', 'Project 2']
          },
          {
            title: 'Development',
            projectNames: ['Project 1', 'Project 2']
          },
          {
            title: 'Automatization',
            projectNames: ['Project 1', 'Project 2']
          },
          {
            title: 'Personal',
            projectNames: ['Project 1', 'Project 2']
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
  justify-content: space-between;
  margin: 5vh 0;
}
</style>