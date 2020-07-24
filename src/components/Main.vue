<template>
<v-app>
    <omnie/>
    <portfolio/>
</v-app>
</template>

<script>
    import omnie from "./omnie";
    import portfolio from "./portfolio";

    export default {
        name: "Main",
        components: {
            omnie,
            portfolio
        },
    }
</script>

<style scoped>

</style>
