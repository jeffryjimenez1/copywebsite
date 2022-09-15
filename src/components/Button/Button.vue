<script setup>

const props = defineProps({
        ctaButton: {
            type: String
        }
    })

</script>

<template>  
    <button :class="main-button" class="cta-button">{{ctaButton}}</button>
</template>

<style scoped>

.cta-button {
display: block;
margin-top: 20px;
padding: 15px 30px;
background: #365A5C;
color: #fff;
border-radius: 5px;
font-size: 1.1rem;
border: none;
box-shadow: 10px 10px 23px -7px rgba(0,0,0,0.75);
-webkit-box-shadow: 10px 10px 23px -7px rgba(0,0,0,0.75);
-moz-box-shadow: 10px 10px 23px -7px rgba(0,0,0,0.75);
}

.cta-button:hover {
    background: #437072;
}



@media screen and (max-width: 480px) {
    .cta-button {
        font-size: 1rem;
        padding: 10px 15px;
        margin: 0;
    }
}


    
</style>