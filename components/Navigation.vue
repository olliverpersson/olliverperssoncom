<template>
    
    <nav>

        <nuxt-link to="/">Om Mig</nuxt-link>
        <nuxt-link to="/portfolio">Portfolio</nuxt-link>
        <a href="https://sliceonline.se"><img src="Slice_Logga_full.svg" style="width: 90px" /></a>

    </nav>

</template>

<style scoped>

    nav {

        display: flex;
        justify-content: space-around;
        background: transparent;
        flex-direction: column;

    }

    a {

        cursor: pointer;
        color: #fff;
        padding: 15px;
        transition: 0.4s;
        text-decoration: none;
        width: 100vw;
        font-weight: bold;
        text-align: center;

    }

    a:hover {

        color: #011C40;
        background: #fff;

    }

    @media screen and (min-width: 650px) {

        nav {

            flex-direction: row;

        }

        a {

            width: 100%;

        }

    }

</style>