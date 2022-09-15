<script setup>
import ServicesItem from './servicesItem.vue';
import About from '../About/About.vue';
import Button from '../Button/Button.vue';

let servicesSection = 'services-section';

const props = defineProps({
       servicesTitle: {
        type: String
       }
    })

</script>

<template>
    <section>
        <div :class="servicesSection">
            <h2 class="services-title">{{servicesTitle}}</h2>
            <ServicesItem 
            addIcon="fa-solid fa-circle-check"
            serviceItemText="crambled it to make a type specimen book. It has survived not only five centuries"
            benefitItem="Benefit"
            ></ServicesItem>
            
            <ServicesItem 
            addIcon="fa-solid fa-circle-check"
            serviceItemText="it look like readable English. Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text"
            benefitItem="Benefit"
            ></ServicesItem>

            <ServicesItem 
            addIcon="fa-solid fa-circle-check"
            serviceItemText="There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour"
            benefitItem="Benefit"
            ></ServicesItem>
            <ServicesItem 
            addIcon="fa-solid fa-circle-check"
            serviceItemText="it look like readable English. Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text"
            benefitItem="Benefit"
            ></ServicesItem>

            <Button ctaButton="I want more information" class="services-button"></Button>

        </div>

        

        <About></About>
    </section>

</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Merriweather&family=Roboto:ital,wght@1,400;1,500&family=Work+Sans&display=swap');


.services-section {
    max-width: 1000px;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-auto-rows: auto repeat(2, 1fr);
    align-content: center;
    justify-content: center;
    font-family: 'Work regular', sans-serif;
    margin: auto;
    grid-gap: 15px;
    padding: 100px 0;
    border-bottom:  5px solid #363A5C;
}

.services-title {
    font-family: 'Work Sans', cursive;
    text-transform: capitalize;
    text-align:  left;
    font-size: 2rem;
    grid-column: 1/3;
    grid-row: 1/2;
    margin-top: 0;
    margin-bottom: 40px;
    color: #5C3636;
}

.services-button {
    margin-top: 50px;
    align-self: center;
    flex-wrap: wrap;
    width: 50%;
}

@media screen and (max-width: 480px) {


    .services-section {
        grid-template-columns: 1fr;
        font-size: 1rem;
        padding: 15px;
        margin: 0;
    }

    .services-title {
        grid-column: 1/2;
        font-size: 1.2rem;
        text-align: left;
        padding: 0 15px;
        margin: 20px 0 10px 0;
    }

    .services-button {
        margin: 20px 0 20px 15px;
    }
}


</style>