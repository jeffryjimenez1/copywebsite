<script setup>
import Header from './components/Header/Header.vue';
import Services from './components/Services/Services.vue';
import Banner from './components/Banner/Banner.vue'
import SupportText from './components/SupportText/SupportText.vue';
import Footer from './components/Footer/Footer.vue';

</script>

<template>
    <Header 
    mainTitle="Text Is Always Relevant"
    subTitle="Professional copywriting speaks to your audience"
    cta="Contact Us"
    ></Header>

    <Services servicesTitle="Convert more interactions"></Services>

    <Banner></Banner>

    <SupportText
    title="Why you need a professional copywriter"

    mainText="Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam quia temporibus harum sunt quo magnam, unde eveniet et mollitia natus dolor ab commodi pariatur architecto accusantium! Perferendis ratione molestias repudiandae."
    ></SupportText>

    <Footer
    title="Our Social Media"
    ></Footer>

</template>



<style scoped>
    body {
        background: #C3E3E1;
    }
</style>
