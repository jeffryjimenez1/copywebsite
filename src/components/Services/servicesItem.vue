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
    font-size: 2rem;
    color: #363A5C;
}

.service-item {
    border-right: 2px solid #363A5C;
    border-bottom:  2px solid #363A5C;
    text-align: left;
    padding: 30px;
    border-radius: 10px;
    font-family: 'Work Sans', sans-serif;
    transition: all 0.2 ease;
    box-shadow: 1px 1px 8px 2px rgba(0,0,0,0.75);
    margin: 20px auto;
}


.service-item-text {
    text-align: left;
    font-size: 1.1rem;
    line-height: 1.6;
    margin-top: 20px;
}

.service-item-text h2 {
    color: #5C3636;
    border-bottom: 1px solid #363A5C;
    margin-bottom: 20px;
    font-size: 1.2rem;
}

@media screen and (max-width: 480px) {
    .myIcon {
        font-size: 1.5rem;
        color: #363A5C;
    }
    .service-item {
        padding: 5px;
        width: 90%;
        box-shadow: none;
    }

    .service-item-text h2 {
        font-size: 1.2rem;
        margin: 10px 0; 
    }

    .service-item-text {
        font-size: 1rem;
        margin: 0;
        padding: 0;
    }

}


</style>