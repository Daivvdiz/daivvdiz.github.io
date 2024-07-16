<template>
<div class="profileContainer">
    <div class="photoContainer">
        <img src="@/assets/icons/Profile.jpg" alt="Profile">
    </div>
    <div class="messageContainer">
        <h3>Hi, I'm David</h3>
    </div>
</div>
</template>


<script>

</script>

<style scoped>
@media screen and (min-width: 1024px){
    .profileContainer {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-top: 5vh;
        padding: 2vh 0;
        max-height: 500px;
    }

    .photoContainer {
        margin-top: 1rem;
        margin-bottom: .5rem;
        border-radius: 50%;
        filter: drop-shadow(0 0 0.4rem #faebd740);
    }

    .photoContainer img {
        max-height: 120px;
        border-radius: 50%;
    }

    .messageContainer h3 {
        font-size: .8rem;
        letter-spacing: 1px;
    }
}

@media screen and (max-width: 1024px){
    .profileContainer {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-top: 5vh;
        padding: 2vh 0;
        max-height: 500px;
    }

    .photoContainer {
        margin-top: 1rem;
        margin-bottom: .5rem;
        border-radius: 50%;
        filter: drop-shadow(0 0 0.4rem #faebd740);
    }

    .photoContainer img {
        max-height: 120px;
        border-radius: 50%;
    }

    .messageContainer h3 {
        font-size: .8rem;
        letter-spacing: 1px;
    }
}
</style>