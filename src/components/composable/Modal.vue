<script setup>
import { stringify } from 'postcss';

let open = false;


</script>

<template>
    <div class="modal">
        <h1>My Modal Form</h1>
        <form class="modal-form">
            <label for="name">Name</label>
            <input type="text" placeholder="Enter your name">
        </form>
    </div>
    
</template> 

<style scoped>

    .modal {
        width: 400px;
        background: black;
        color: #fff;
        position: fixed;
    }

</style>