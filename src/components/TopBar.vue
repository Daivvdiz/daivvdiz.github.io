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
.topContainer {
    border-bottom: 1px solid #9e9e9eb3;
    display: flex;
    justify-content: space-evenly;
    width: 100%;
    height: 10vh;
    padding: 0 1rem
}

.topContainer>div {
    display: flex;
    width: 50%;
    align-items: center;
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
}

.mailContainer img {
    width: 2vh
}

.rightContainer {
    display: flex;
    justify-content: end;
}

.rightContainer img {
    width: 2vh;
    margin: 0 1rem;
}

</style>