<template>
    <div class="cardContainer">
        <div class="topicCard">
        <h1>{{ name }}</h1>
            <div class="projectsContainer">
                <ul>
                    <li v-for="(content, index) in contents" :key="index"><a :href="routeProfile[index]" target="_blank">{{ '→ '+content }}</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props: {
            name: {
                type: String,
                required: true
            },
            contents: {
                type: Array,
                required: true
            },
            routeProfile: {
                type: Array,
                required: false,
            }
        }
    };
</script>

<style scoped>

@media (min-width: 1024px) {
    .cardContainer {
        font-family: "Josefin Sans", sans-serif;
        display: flex;
        flex-direction: column;
        padding: 1px;
        background-color: #FFFFFF;
        border-radius: 1rem;
        width: 20%;
    }
    
    .topicCard {
        background: #1A1A1A;
        padding: 0 1rem;
        padding-top: 2rem;
        min-height: 280px;
        border-radius: 1rem;
        box-shadow: 0 0 10px 1px #ffffff59 inset;
    }

    .topicCard h1 {
        font-size: 1.2rem;
        color: #9E9E9E;
        font-weight: 600;
    }

    .topicCard ul {
        display: flex;
        flex-direction: column;
        text-align: start;
        justify-content: start;
        margin-top: 1rem;
        padding-right: 1.5rem;
    }

    .topicCard li {
        list-style: none;
        margin: 0.5rem 0;
        margin-left: .2rem;
    }

    .topicCard a {
        color: hsla(0, 0%, 96%, 0.4);
        font-size: .85rem;
        font-weight: 400;
        display: flex;
        width: 100%;
        text-decoration: none;
        cursor: pointer;
        padding: 0 .5rem;
        border-radius: 5px;
    }

    .topicCard a:hover {
        background-color: #9E9E9E;
        color: #1A1A1A;
    }
}

@media (max-width: 1024px) {
    .cardContainer {
        font-family: "Josefin Sans", sans-serif;
        display: flex;
        flex-direction: column;
        padding: 1px;
        background-color: #FFFFFF;
        border-radius: 1rem;
        min-width: 250px;
        margin: 0 4rem;
    }
    
    .topicCard {
        background: #1A1A1A;
        padding: 0 1rem;
        padding-top: 2rem;
        min-height: 280px;
        border-radius: 1rem;
        box-shadow: 0 0 10px 1px #ffffff59 inset;
    }

    .topicCard h1 {
        font-size: 1.2rem;
        color: #9E9E9E;
        font-weight: 600;
    }

    .topicCard ul {
        display: flex;
        flex-direction: column;
        text-align: start;
        justify-content: start;
        margin-top: 1rem;
        padding-right: 1.5rem;
    }

    .topicCard li {
        list-style: none;
        margin: 0.5rem 0;
        margin-left: .2rem;
    }

    .topicCard a {
        color: hsla(0, 0%, 96%, 0.4);
        font-size: .85rem;
        font-weight: 400;
        display: flex;
        width: 100%;
        text-decoration: none;
        cursor: pointer;
        padding: 0 .5rem;
        border-radius: 5px;
    }

    .topicCard a:hover {
        background-color: #9E9E9E;
        color: #1A1A1A;
    }
}
</style>