<template>
    <div class="carouselContainer">
        <div class="iconsContainer">
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
    </div>
</template>

<script>

</script>

<style scoped>

@media screen and (min-width: 1024px){
    .carouselContainer {
        background: linear-gradient(to right, #161616, #f9e7ce, #161616);
        padding: 1px 0;
        margin: 15vh 0;
    }
    
    .iconsContainer {
        background-color: #161616;
        display: flex;
        height: 100%;
        padding: 2rem;
        align-items: center;
        justify-content: space-around;
    }
    
    .iconsContainer img {
        max-width: 200px
    }
}


</style>