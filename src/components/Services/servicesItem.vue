<script setup>

let myIcon = 'myIcon';

const props = defineProps({
        addIcon: {
            type: String
        },
        serviceItemText: {
            type: String
        },
        benefitItem: {
            type: String
        }
    })
</script>

<template>  
        <div class="service-item">
            <div class="service-img">
                <i :class="addIcon" class="myIcon"></i>
            </div>
            <div class="service-item-text">
                <h2>{{benefitItem}}</h2>
                <p>{{serviceItemText}}</p>
            </div>
        </div>
</template>

<style scoped>

.myIcon {
    font-size: 50px;
    color: #363A5C;
}

.service-item {
    border-right: 5px solid #363A5C;
    border-bottom:  5px solid #363A5C;
    text-align: left;
    padding: 30px;
    border-radius: 10px;
    font-family: 'Work Sans', sans-serif;
    transition: all 0.2 ease;
    box-shadow: 10px 10px 23px -7px rgba(0,0,0,0.75);
-webkit-box-shadow: 10px 10px 23px -7px rgba(0,0,0,0.75);
-moz-box-shadow: 10px 10px 23px -7px rgba(0,0,0,0.75);
}


.service-item-text {
    text-align: left;
    font-size: 1.3rem;
    line-height: 1.6;
    margin-top: 20px;
}

.service-item-text h2 {
    color: #5C3636;
}


</style>