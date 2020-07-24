<template>
    <v-container-fluid>
        <v-toolbar
                app
                dark

        >
            <v-app-bar-nav-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-app-bar-nav-icon>
            <v-toolbar-title>
                <h2
                        class="navbar-title"
                >Daniel Sobieraj</h2>
            </v-toolbar-title>

            <v-spacer></v-spacer>
            <v-toolbar-items class="hidden-sm-and-down">
                <v-btn
                        target="_blank"
                        text
                        rounded
                >
                    <span class="mr-2">O mnie</span>
                </v-btn>
                <v-btn
                        text
                        rounded
                >
                    <span class="mr-2">Portfolio</span>
                </v-btn>
                <v-btn
                        href="/omnie"
                        target="_blank"
                        text
                        rounded
                >
                    <span class="mr-2">Kontakt</span>
                </v-btn>
            </v-toolbar-items>
        </v-toolbar>

        <v-navigation-drawer
                v-model="drawer"
                class="v-navigation-drawer--absolute"
                dark>
            <v-btn
                    target="_blank"
                    text
                    rounded
            >
                <span class="mr-2">O mnie</span>
            </v-btn>
            <v-btn
                    text
                    rounded
            >
                <span class="mr-2">Portfolio</span>
            </v-btn>
            <v-btn
                    href="/omnie"
                    target="_blank"
                    text
                    rounded
            >
                <span class="mr-2">Kontakt</span>
            </v-btn>
        </v-navigation-drawer>
    </v-container-fluid>
</template>

<script>
    export default {
        name: 'NavBar',
        data() {
            return {
                drawer: false
            }
        }
    }
</script>

<style lang="css">
    .navbar-title {
        font-weight: 400;
        Size: 6rem;
        letter-spacing: .1rem;
    }

    .v-navigation-drawer__content {
        height: 30vh!important;
        display: flex;
        flex-direction: column;
        justify-content: space-around
    }
</style>
