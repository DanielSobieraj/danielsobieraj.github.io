<template>
    <v-app-bar
            app
            color="primary"
            dark

    >
        <div class="d-flex align-center">
            <v-img
                    alt="Vuetify Logo"
                    class="shrink mr-3"
                    contain
                    src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/1184px-Vue.js_Logo_2.svg.png"
                    transition="scale-transition"
                    width="40"
            />

            <h1>Daniel Sobieraj</h1>
        </div>

        <v-spacer></v-spacer>

        <v-btn
                href="https://github.com/vuetifyjs/vuetify/releases/latest"
                target="_blank"
                text
        >
            <span class="mr-2">O mnie</span>
        </v-btn>
        <v-btn
                href="https://github.com/vuetifyjs/vuetify/releases/latest"
                target="_blank"
                text
        >
            <span class="mr-2">Portfolio</span>
        </v-btn>
        <v-btn
                href="https://github.com/vuetifyjs/vuetify/releases/latest"
                target="_blank"
                text
        >
            <span class="mr-2">Kontakt</span>
        </v-btn>
        <v-app-bar-nav-icon
            class="d-md-none"
        >
            <v-btn
                    href="https://github.com/vuetifyjs/vuetify/releases/latest"
                    target="_blank"
                    text
            >
                <span class="mr-2">O mnie</span>
            </v-btn>
            <v-btn
                    href="https://github.com/vuetifyjs/vuetify/releases/latest"
                    target="_blank"
                    text
            >
                <span class="mr-2">Portfolio</span>
            </v-btn>
            <v-btn
                    href="https://github.com/vuetifyjs/vuetify/releases/latest"
                    target="_blank"
                    text
            >
                <span class="mr-2">Kontakt</span>
            </v-btn>
        </v-app-bar-nav-icon>
    </v-app-bar>
</template>

<script>
    export default {
        name: "Navbar"
    }
</script>

<style scoped>
h1 {
    font-family: Roboto,serif;
    font-weight: 300;
    Size: 6rem;
    letter-spacing: .1rem;
}
</style>
