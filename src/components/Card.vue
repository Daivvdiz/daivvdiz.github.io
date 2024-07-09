<template>
    <div class="topicCard">
        <h1>{{ title }}</h1>
        <div class="projectsContainer">
            <ul>
                <li v-for="(projectName, index) in projectNames" :key="index"><a href="">{{ projectName }}</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        props: {
            title: {
                type: String,
                required: true
            },
            projectNames: {
                type: Array,
                required: true
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
    }

    .topicCard a {
        color: #9e9e9e66;
        font-size: 1rem;
        font-weight: 600;
        display: flex;
        width: 100%;
        text-decoration: none;
    }

    .topicCard a:hover {
        background-color: #9E9E9E;
        color: #1A1A1A;
    }
}
</style>