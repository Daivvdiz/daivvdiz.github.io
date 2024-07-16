<template>
    <div class="bottomBarContainer">
        <div class="infoContainer">
            <h2>Contact Me</h2>
            <div class="mailContainer">
                <img src="@/assets/icons/Mail.png" alt="Mail">
                <h3>daivvdiz@gmail.com</h3>
            </div>
            <div class="linkedinContainer">
                <a href="https://www.linkedin.com/in/daivvdiz/" target="_blank"><img src="@/assets/icons/Linkedin.png" alt="Linkedin"></a>
                <h3>https://www.linkedin.com/in/daivvdiz/</h3>
            </div>
            <div class="gitHubContainer">
                <a href="https://github.com/daivvdiz" target="_blank"><img src="@/assets/icons/GitHub.png" alt="GitHub"></a>
                <h3>https://github.com/daivvdiz</h3>
            </div>
            <div class="instaContainer">
                <a href="https://www.instagram.com/daivdiz/" target="_blank"><img src="@/assets/icons/Instagram.png" alt="Instagram"></a>
                <h3>https://www.instagram.com/daivdiz/</h3>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style scoped>
@media screen and (max-width: 1024px){
    .bottomBarContainer {
        background-image: linear-gradient(to bottom, #18181800, #181818);
        display: flex;
        justify-content: start;
        width: 100%;
    }

    .infoContainer {
        margin-left: 5rem;
    }

    .infoContainer>div {
        display: flex;
        margin: 1rem 0;
        align-items: center;
        justify-content: start;
    }
    
    .infoContainer h2 {
        margin-bottom: 2rem;
        font-weight: bold;
    }

    .infoContainer div h3 {
        font-weight: lighter;
        margin-left: 1rem;
    }

    .infoContainer div img {
        width: 20px;
        filter: opacity(.6)
    }
}
</style>