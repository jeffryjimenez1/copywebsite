<script setup>
import Header from './components/Header/Header.vue';
import Services from './components/Services/Services.vue';
import Banner from './components/Banner/Banner.vue'

</script>

<template>
    <Header 
    mainTitle="Text Is Always Relevant"
    subTitle="Professional copywriting speaks to your audience"
    cta="Contact Us"
    ></Header>

    <Services servicesTitle="Convert more interactions"></Services>

    <Banner></Banner>

</template>



<style scoped>
    body {
        background: #C3E3E1;
    }
</style>
