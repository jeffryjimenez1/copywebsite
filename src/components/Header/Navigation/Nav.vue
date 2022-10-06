<script setup>
    
    import NavItems from './NavItems.vue'

    let navList = 'main-nav-list'
    let hideList = 'hidden'
    let mainNav = 'main-nav'
    let isActive = true;
    const hamburgerBtn = 'hamburger-menu'

    function useNavBtn(e) {
       document.querySelector('.main-nav-list').classList.toggle('hidden');
    }

</script>

<template>
    
    <nav :class="mainNav">
        <ul :class="navList">
            <li class="logo">Jeff | Copywriter</li>
            <NavItems linkName="#home" class="homeLink">Home</NavItems>
            <NavItems linkName="#contact">Contact</NavItems>
            <NavItems linkName="#services">Services</NavItems>
        </ul>
        <div @click="useNavBtn" :class="hamburgerBtn">
            <div class="line line1"></div>
            <div class="line line2"></div>
            <div class="line line3"></div>
        </div>
    </nav>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500&family=Oleo+Script&family=Roboto+Condensed&family=Roboto:ital,wght@1,500&display=swap');

html {
    margin: 0;
    padding: 0;
}

.main-nav-list {
    display: flex;
    justify-content: flex-end;
    border-bottom: 3px solid black;
    margin: 0;
    font-family: 'Work Sans', sans-serif;
}

.logo {
    list-style: none;
    align-self: center;
    margin-right: auto;
    padding: 20px 40px;
}


@media screen and (max-width: 480px) {

    .hidden {
        transform: translate(100%);
    }
    .main-nav-list {
        position: fixed;
        left: -100%;
        z-index: 10;
        flex-direction: column;
        justify-content: center;
        width: 100%;
        height: 100vh;
        background-image: linear-gradient(to right top, #365c3a, #01584e, #00515f, #0b4764, #363a5c);
        transition: translate 1 ease;
    }
    
    .hamburger-menu {
        display: block;
        position: fixed;
        border: 1px solid black;
        padding: 3px;
        right: 10px;
        top: 10px;
        border-radius: 5px;
        z-index: 30;
    }

    .line {
        width: 30px;
        height: 5px;
        background: #000;
    }

    .line2 {
        margin: 5px 0;
    }

}

</style>