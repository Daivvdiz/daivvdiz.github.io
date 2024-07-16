<template>
    <div class="carouselContainer">
        <div class="iconContainer">
            <div class="iconItem">
                <a href="https://emcocables.co/" target="_blank"><img src="@/assets/icons/Emcocables.png" alt="Emcocables"></a>
            </div>
            <div class="iconItem">
                <a href="https://www.usbbog.edu.co/" target="_blank"><img src="@/assets/icons/Universidad.png" alt="Universidad"></a>
            </div>
            <div class="iconItem">
                <a href="https://www.sena.edu.co/es-co/Paginas/default.aspx" target="_blank"><img src="@/assets/icons/Sena.png" alt="SENA"></a>
            </div>
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

    .carouselContainer a:hover {
        filter: invert(.4)
    }

    .carouselContainer a img {
        max-height: 80px;
        margin: 0 2rem;
    }
}

@media screen and (max-width: 1024px){
    .carouselContainer {
        display: flex;
        width: 100%;
        align-items: center;
        padding: 5rem 0;
    }

    .iconContainer {
        display: flex;
        width: 100%;
        overflow-x: scroll;
    }

    .iconItem {
        display: flex;
        width: 400px;
        margin: 0 3rem;
        justify-content: center;
        align-items: center;
    }

    .iconContainer a {
        display: flex;
        height: 100%;
        margin: 0 5rem;
    }

    .carouselContainer a:hover {
        filter: invert(.4);
    }

    .carouselContainer a img {
        max-height: 80px;
        margin: 0 2rem;
    }
}

</style>