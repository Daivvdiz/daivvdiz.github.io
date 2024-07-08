<script setup>
import TopBar from '../components/TopBar.vue';
import Profile from '../components/Profile.vue';
import Slogan from '../components/Slogan.vue';
</script>

<template>
  <main>
    <TopBar />
    <Profile />
    <Slogan textSlogan="Versatility and curiosity: exploring without limits."/>
    
    <Slogan textSlogan="A journey of constant evolution"/>
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