<script setup>


</script>
    
<template>  
    <div class="banner">
        <div class="banner-text">
            <h1>Is your audience engaging with you?</h1>
        </div>
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Merriweather&family=Roboto:ital,wght@1,400;1,500&family=Work+Sans&display=swap');


.banner {
    width: 100%;
    text-align: center;
    background-image: linear-gradient(to right top, #365c3a, #01584e, #00515f, #0b4764, #363a5c);    height: 30vh;
    color: #FCFAFB;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Work Sans', sans-serif;
    padding: 100px 0;
}

.banner h1{
    font-size: 3rem;
}

@media screen and (max-width: 480px) {

    .banner {
        padding: 20px 0;
    }
    .banner h1{
        font-size: 1.3rem;
    }
}
</style>