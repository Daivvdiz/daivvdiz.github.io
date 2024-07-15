<template>
    <div class="topContainer">
        <div class="leftContainer">
            <div class="mailContainer">
                <img src="./icons/Mail.png" alt="Mail">
                <h3>daivvdiz@gmail.com</h3>
            </div>
        </div>
        <div class="rightContainer">
            <img src="./icons/Linkedin.png" alt="Linkedin">
            <img src="./icons/GitHub.png" alt="GitHub">
            <img src="./icons/Instagram.png" alt="Instagram">
        </div>
    </div>
</template>


<script>
export default {

}
</script>

<style scoped>
@media screen and (min-width: 1024px){
    .topContainer {
        border-bottom: 1px solid #FFFFFF;
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        width: 70%;
        height: 100%;
        max-height: 90px;
        padding: 1rem 0;
    }
    
    .topContainer>div {
        display: flex;
        width: 50%;
        align-items: center;
        margin-top: -1rem
    }
    
    .leftContainer {
        display: flex;
        justify-content: start;
    }
    
    .mailContainer {
        display: flex;
        align-items: center;
    }
    
    .mailContainer h3 {
        margin-left: 1rem;
        font-size: .8rem;
        font-weight: 300;
        letter-spacing: 1px;
    }

    .rightContainer {
        display: flex;
        justify-content: end;
        padding-right: 2rem;
    }
    
    .mailContainer img, .rightContainer img {
        width: 2.5vh;
        margin-left: 1rem;
    }
}
</style>