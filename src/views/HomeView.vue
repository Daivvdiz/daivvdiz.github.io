<script setup>
import TopBar from '../components/TopBar.vue';
import Profile from '../components/Profile.vue';
import Slogan from '../components/Slogan.vue';
import Carousel from '../components/Carousel.vue';
import TopicCards from '../components/TopicCards.vue';
</script>

<template>
  <main>
    <TopBar />
    <Profile />
    <Slogan textSlogan="Versatility and curiosity: exploring without limits."/>
    <Carousel />
    <Slogan textSlogan="A journey of constant evolution"/>
    <TopicCards />
  </main>
</template>

<script>
  export default {
    name: 'HomeView',
    components: {
      Slogan,
    },
  };
</script>