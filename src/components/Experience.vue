<template>
    <div class="carouselContainer">
        <div class="iconItem">
            <img src="./icons/Emcocables.png" alt="Emcocables">
        </div>
        <div class="iconItem">
            <img src="./icons/Universidad.png" alt="Universidad">
        </div>
        <div class="iconItem">
            <img src="./icons/Sena.png" alt="SENA">
        </div>
    </div>
</template>

<script>

</script>

<style scoped>

@media screen and (min-width: 1024px){
    .carouselContainer {
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        padding: 3rem 0;
    }
    
    .carouselContainer img {
        max-height: 80px;
        margin: 0 2rem;
    }
}


</style>