<template>
    <div class="aboutMeButtonContainer">
        <div class="buttonContainer">
            <div class="textContainer">
                <h2>About Me</h2>
                <img src="./icons/Link.png" alt="Link">
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style scoped>
@media screen and (min-width: 1024px){
    
    .buttonContainer {
        border: 2px solid #ffffff66;
        border-radius: 2px;
        padding: 1px;
        opacity: 0.4;
        transition: opacity .15s ease-out;
    }

    .buttonContainer:hover {
        opacity: 1;
        cursor: pointer;
    }

    .textContainer {
        background-color: hsla(0, 0%, 9%, 0.5);
        border-radius: 5px;
        display: flex;
        padding: 1rem .2rem;
        justify-content: center;
        align-items: center;
    }
    
    .textContainer>* {
        margin: 0 .5rem;
    }

    .textContainer img {
        margin-top: -.3rem;
        max-height: 1rem;
        rotate: -50deg;
    }
}
</style>