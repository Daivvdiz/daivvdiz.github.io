<template>
    <div class="topicCard">
        <h1>{{ name }}</h1>
        <div class="projectsContainer">
            <ul>
                <li v-for="(content, index) in contents" :key="index"><a :href="routeProfile[index]" target="_blank">{{ '→ '+content }}</a></li>
            </ul>
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
    .topicCard {
        font-family: "Josefin Sans", sans-serif;
        background: #1A1A1A;
        border: 2px solid #9e9e9e66;
        padding: 2rem 10px;
        width: 20%;
        min-height: 280px;
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
        margin-top: 2rem;
    }

    .topicCard li {
        list-style: none;
        margin: 0.5rem 0;
        margin-left: .2rem;
    }

    .topicCard a {
        color: #9e9e9e66;
        font-size: 1rem;
        font-weight: 600;
        display: flex;
        width: 100%;
        text-decoration: none;
        cursor: pointer;
    }

    .topicCard a:hover {
        background-color: #9E9E9E;
        color: #1A1A1A;
        /* cursor: pointer; */
    }
}
</style>