<script setup>
import TopBar from '../components/TopBar.vue';
import Profile from '../components/Profile.vue';
import AboutMeButton from '../components/AboutMeButton.vue';
import RelevantText from '../components/RelevantText.vue';
import Experience from '../components/Experience.vue';
import CardListProjects from '../components/CardListProjects.vue';
import CardListStudy from '../components/CardListStudy.vue';
</script>

<template>
  <main>
    <TopBar />
    <Profile />
    <!-- <AboutMeButton /> -->
    <RelevantText :relevantText="'Versatility and curiosity: exploring without\nlimits.'"/>
    <Experience />
    <RelevantText :relevantText="'A journey of constant evolution'"/>
    <CardListProjects/>
    <RelevantText :relevantText="'Lifelong learning: embracing knowledge at \nevery step'" />
    <CardListStudy />
  </main>
</template>

<style scoped>
@media screen and (min-width: 1024px){
  main {
    background-color: rgba(0, 0, 0, 0.85);
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

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

<script>
  export default {
    name: 'HomeView',
    components: {
      Slogan: RelevantText,
    }
  };
</script>