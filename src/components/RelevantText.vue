<template>
    <div class="sloganContainer">
        <h2 v-html="formattedText"></h2>
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
    computed:{
      formattedText() {
        return this.relevantText.replace(/\n/g, '<br />');
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
  }

  .sloganContainer h2 {
    font-size: 3rem;
    padding: 1rem;
    text-align: center;
    background: -webkit-linear-gradient(275deg,#9E9E9E 0%, #F4F4F4 70%,#9E9E9E 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
}
</style>