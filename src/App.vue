<template>
    <v-app>
        <Navbar/>
        <Hero/>
        <Main/>
    </v-app>
</template>

<script>
    import Navbar from "./components/Navbar";
    import Hero from './components/Hero';
    import Main from "./components/Main";

    export default {
        name: 'App',

        components: {
            Navbar,
            Hero,
            Main
        },

        data: () => ({
            //
        }),
    };
</script>

<style lang="scss">
    @import url('https://fonts.googleapis.com/css2? family=Open+Sans&display=swap');

    $body-font-family: 'Open Sans';

    #app, h2 {
        font-family: $body-font-family, sans-serif !important;
    }

    .v-application {
        font-family: $body-font-family, sans-serif !important;
    }
</style>
