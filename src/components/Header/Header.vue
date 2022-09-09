<script setup>
    import Nav from './Navigation/Nav.vue'
import Button from '../Button/Button.vue';

    const props = defineProps({
        mainTitle: {
                type: String            
            },
        subTitle: {
            type: String
        },
        cta: {
            type: String
        }
    })

    const mainHeader = "main-header";
    const showcase = 'showcase';
    const showcaseText = 'showcase-text';
    const ctaButton = 'main-button'


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
    </header>
</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Merriweather&family=Roboto:ital,wght@1,400;1,500&family=Work+Sans&display=swap');


.main-header {
    max-width: 1200px;
    margin: auto;
    font-size: 1.3rem;
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
}

.showcase-text h1 {
    margin-bottom: 40px;
    font-family: 'Work Sans', cursive;
    text-align: left;
    font-size: 4rem;
    color: #5C3636;
}

span {
    font-family: 'Work Sans', sans-serif;
    display: block;
    margin: 50px 0;
}


</style>