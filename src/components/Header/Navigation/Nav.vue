<script setup>
    
    import NavItems from './NavItems.vue'

    let mainNav = 'main-nav'

</script>

<template>
    <nav :class="mainNav">
        <ul>
            <NavItems logo="logo">Influential Words</NavItems>
            <NavItems linkName="#home">Copywriting Services</NavItems>
            <NavItems linkName="#contact">Contact</NavItems>
            <NavItems linkName="#services">Services</NavItems>
        </ul>
    </nav>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500&family=Oleo+Script&family=Roboto+Condensed&family=Roboto:ital,wght@1,500&display=swap');

html {
    margin: 0;
    padding: 0;
}
.main-nav ul {
    display: flex;
    justify-content: flex-end;
    border-bottom: 3px solid black;
    margin: 0;
    font-family: 'Work Sans', sans-serif;
}

</style>