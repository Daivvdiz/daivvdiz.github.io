<template>
    <div class="sloganContainer">
        <h2>{{ relevantText }}</h2>
    </div>
</template>

<script>
  export default {
    props: {
      relevantText: {
        type: String,
        required: true,
      }
    },
  };
</script>

<style scoped>
@media screen and (min-width: 1024px){
  .sloganContainer {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1rem 0;
    /* max-width: 50%; */
  }

  .sloganContainer h2 {
    font-size: 3rem;
    padding: 1rem;
    text-align: center;
    background: -webkit-linear-gradient(275deg, #f8e6cc 70%,#ffffff 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
}
</style>