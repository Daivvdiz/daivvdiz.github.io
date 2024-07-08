<template>
    <div class="sloganContainer">
        <h2>{{ textSlogan }}</h2>
    </div>
</template>

<script>
  export default {
    props: {
      textSlogan: {
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
        margin-top: 5vh;
        padding: 5vh 0;
    }

    .sloganContainer h2 {
        font-family: "Josefin Sans", sans-serif;
        font-size: 3rem;
        background: -webkit-linear-gradient(275deg, #f9e7ce, #6c6c6c);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        text-align: center;
    }
}
</style>