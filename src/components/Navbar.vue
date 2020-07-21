<template>
    <v-app-bar
            app
            dark

    >
        <div class="d-flex align-center ml-5">
            <h1
                    class="navbar-title"
            >Daniel Sobieraj</h1>
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
        name: 'NavBar',
        data() {
            return {

            }
        }
    }
</script>

<style scoped>
    .navbar-title {
        font-family: Roboto, serif;
        font-weight: 400;
        Size: 6rem;
        letter-spacing: .1rem;
    }
</style>
