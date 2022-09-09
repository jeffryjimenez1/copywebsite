<script setup>

    let navOptions = 'list-item';
    let navLinks = 'link-item';

    const props = defineProps({
        logo: {
            type: String
        },
        linkName: {
            type: String
        }
    })

</script>

<template>
    <li :class="navOptions"><a :href="linkName" :class="navLinks"><slot></slot></a></li>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500&family=Oleo+Script&family=Roboto+Condensed&family=Roboto:ital,wght@1,500&display=swap');

.list-item {
    list-style: none;
}

.list-item:first-child {
    margin-right: auto;
}

.link-item {
    display: inline-block;
    padding: 20px 40px;
    text-decoration: none;
    color: #363A5C;
    transition: all 0.2s ease;
}

.link-item:hover {
    background: #5C3636;
    color: #FCFAFB;
}

</style>