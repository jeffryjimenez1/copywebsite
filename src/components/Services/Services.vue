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
            <h1 class="services-title">{{servicesTitle}}</h1>
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
    max-width: 1200px;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-auto-rows: auto repeat(2, 1fr);
    align-content: center;
    justify-content: center;
    font-family: 'Roboto regular', sans-serif;
    margin: auto;
    grid-gap: 15px;
    padding: 200px 0;
    border-bottom:  5px solid #363A5C;
}

.services-title {
    font-family: 'Work Sans', cursive;
    text-transform: capitalize;
    text-align:  left;
    font-size: 50px;
    grid-column: 1/5;
    grid-row: 1/2;
    margin-top: 0;
    margin-bottom: 40px;
    color: #5C3636;
}

.services-button {
    margin-top: 50px;
}

</style>