<script setup>
    import Nav from './Navigation/Nav.vue'
    import Button from '../Button/Button.vue';
    import { onMounted } from 'vue';

    const props = defineProps({
        mainTitle: {
                type: String            
            },
        subTitle: {
            type: String
        },
        cta: {
            type: String
        },
    })


    const mainHeader = "main-header";
    const showcase = 'showcase';
    const showcaseText = 'showcase-text';
    const ctaButton = 'main-button';
   
    
</script>

<template>      
    <header :class="mainHeader">

        <Nav></Nav>
        <div :class="showcase">
            <div :class="showcaseText">
                <h1>{{mainTitle}}</h1>
                <span>{{subTitle}}</span>
                <Button ctaButton="I need a copywriter"></Button>
            </div>  
        </div>
        <img src="@/assets/img/services1.jpg" class="header-img">
        <img src="@/assets/img/services2.jpg" class="second-img">
    </header>
</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Merriweather&family=Roboto:ital,wght@1,400;1,500&family=Work+Sans&display=swap');


.main-header {
    max-width: 1000px;
    margin: auto;
    font-size: 1.1rem;
    position: relative;
    color: #363A5C;
    border-bottom: 3px solid black;
}


.showcase {
    height: calc(100vh - 66px);
}

.showcase-text {
    position: absolute;
    top: 50%;
    left: 0;
    transform: translate( 0, -50%);
    margin: auto;
    text-align: left;
    z-index: 2;
}

.showcase-text h1 {
    margin-bottom: 40px;
    font-family: 'Work Sans', cursive;
    text-align: left;
    font-size: 3rem;
    color: #5C3636;
}

span {
    font-family: 'Work Sans', sans-serif;
    display: block;
    margin: 50px 0;
}

.header-img {
    position: absolute;
    object-fit: cover;
    width: 250px;
    height: 250px;
    top: 60%;
    transform: translateY(-50%);
    right: 20%;
    z-index: 1;
    border-radius: 10px;
}

.second-img {
    position: absolute;
    object-fit: cover;
    width: 250px;
    height: 250px;
    top: 40%;
    transform: translateY(-50%);
    right: 0;
    z-index: 1;
    border-radius: 10px;
}

@media screen and (max-width: 480px) {


    .main-header {
        padding: 0 15px;
        font-size: 1.1rem;
        margin: 0 auto;
        height: 100vh;
    }

    .main-header img {
        display: none;
    }

    .showcase {
        width: 80%;
    }

    span {
       font-size: 1rem;
       margin: 30px 0;
    }



    .showcase-text {
        width: 80%;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
    }

    .showcase-text h1 {
        font-size: 2rem;
        margin-bottom: 25px;
    }
}
</style>