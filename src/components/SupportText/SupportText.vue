<script setup>

const props = defineProps({
        title: {
            type: String
        },
        mainText: {
            type: String
        }
    })

</script>

<template>

<section class="supportText">
    
    <div class="supporContent">
        <h1>{{title}}</h1>
        <p>{{mainText}}</p>

    </div>
</section>



</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Merriweather&family=Roboto:ital,wght@1,400;1,500&family=Work+Sans&display=swap');

.supportText {
    max-width: 1000px;
    margin: auto;
    font-family: 'Work Sans', sans-serif;
}

h1 {
    font-size: 2rem;
    color: #5C3636;
    margin-bottom: 40px;
}

.supporContent {
    width: 50%;
    font-size: 1.1rem;
    padding: 100px 0;
    color: #363A5C;
}

@media screen and (max-width: 480px) {

    .supportText {
        padding: 15px;
        width: 90%;
        font-size: 1.3rem;
        margin: 0;
    }
    .supporContent {
        width: 100%;
        font-size: 1.1rem;
        color: #363A5C;
        margin: 0;
    }
}
</style>