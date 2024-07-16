<script setup>
import TopBar from '../components/TopBar.vue';
import Profile from '../components/Profile.vue';
import RelevantText from '../components/RelevantText.vue';
import Experience from '../components/Experience.vue';
import CardListProjects from '../components/CardListProjects.vue';
import CardListStudy from '../components/CardListStudy.vue';
import BottomBar from '../components/BottomBar.vue';
</script>

<template>
  <main>
    <TopBar v-if="showBar"/>
    <Profile />
    <RelevantText :relevantText="'Versatility and curiosity: exploring without\nlimits.'"/>
    <Experience />
    <RelevantText :relevantText="'A journey of constant evolution'"/>
    <CardListProjects/>
    <RelevantText :relevantText="'Lifelong learning: embracing knowledge at \nevery step'" />
    <CardListStudy />
    <BottomBar v-if="!showBar"/>
  </main>
</template>

<style scoped>
main {
  background-color: rgba(0, 0, 0, 0.85);
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

@media screen and (min-width: 1024px){
  main>* {
    height: calc(100vh/7);
    width: 100%;
    max-width: 1280px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 1.2rem 0;
    /* background-color: rgba(128, 0, 128, 0.445); */
  }
}
</style>

<style>
@media screen and (max-width: 1024px){
  .topicCardsContainer {
    display: flex;
    width: 100%;
    padding: 3rem 0;
    justify-content: center;
    overflow: hidden;
  }

  .listCardContainer{
    display: flex;
    overflow-x: scroll;
  }
}
</style>

<script>
  export default {
    name: 'HomeView',
    components: {
      Slogan: RelevantText,
      TopBar,
    },
    data() {
      return {
        windowWidth: window.innerWidth
      };
    },
    computed: {
      showBar() {
        return this.windowWidth > 1023;
      }
    },
    created() {
      window.addEventListener('resize', this.handleResize);
    },
    beforeDestroy() {
      window.removeEventListener('resize', this.handleResize);
    },
    methods: {
      handleResize() {
        this.windowWidth = window.innerWidth;
      }
    }
  };
</script>