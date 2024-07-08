<template>
<div class="profileContainer">
    <div class="photoContainer">
        <img src="./icons/Profile.png" alt="Profile">
    </div>
    <div class="messageContainer">
        <h3>Hi, I'm David 👋</h3>
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
        margin: 1.5rem 0;
        border-radius: 50%;
        filter: drop-shadow(0 0 0.4rem #faebd740);
    }

    .photoContainer img {
        max-width: 150px;
        border-radius: 50%;
    }
}
</style>