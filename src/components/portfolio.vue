<template>
    <v-container>
        <v-row>
            <v-col>
                <h2 class="mb-4">Portfolio</h2>
                <div class="d-flex justify-space-around flex-wrap">
                    <v-hover v-slot:default="{ hover }">
                        <v-card
                                :elevation="hover ? 12 : 2"
                                :class="{ 'on-hover': hover }"
                                max-width="400"
                        >
                            <v-img
                                    class="white--text align-end"
                                    height="200px"
                                    src="../assets/fortpiaski.png"
                            >
                            </v-img>

                            <v-card-subtitle>Strona wizytówka<br>Fort Piaski</v-card-subtitle>

                            <v-card-text class="text--primary d-flex justify-space-around">
                                <img src="https://image.flaticon.com/icons/svg/1216/1216733.svg" alt="" height="32px">
                                <img src="https://image.flaticon.com/icons/svg/732/732190.svg" alt="" height="32px">
                                <img src="https://image.flaticon.com/icons/svg/919/919828.svg" alt="" height="32px">
                                <img src="https://image.flaticon.com/icons/svg/174/174881.svg" alt="" height="32px">
                                <img src="https://image.flaticon.com/icons/svg/919/919830.svg" alt="" height="32px">
                            </v-card-text>

                            <v-card-actions>
                                <v-btn
                                        text
                                        rounded
                                >
                                    Link
                                </v-btn>

                            </v-card-actions>
                        </v-card>
                    </v-hover>
                    <v-hover v-slot:default="{ hover }">
                        <v-card
                                :elevation="hover ? 12 : 2"
                                :class="{ 'on-hover': hover }"
                                max-width="400"
                        >
                            <v-img
                                    :class="{ 'on-hover': hover }"
                                    class="white--text align-end"
                                    height="200px"
                                    src="../assets/twojemodele.png"
                            >
                                <v-card-actions>
                                    <v-btn
                                            text
                                            rounded
                                            color="transparent"
                                            :class="{ 'show-btns': hover }"
                                    >
                                        Link
                                    </v-btn>
                                </v-card-actions>
                            </v-img>

                            <v-card-subtitle>Sklep internetowy<br>Twoje-modele.pl</v-card-subtitle>

                            <v-card-text class="text--primary d-flex justify-space-around">
                                <img src="https://image.flaticon.com/icons/svg/1216/1216733.svg" alt="" height="32px">
                                <img src="https://image.flaticon.com/icons/svg/732/732190.svg" alt="" height="32px">
                                <img src="https://image.flaticon.com/icons/svg/825/825533.svg" alt="" height="32px">
                            </v-card-text>
                        </v-card>
                    </v-hover>
                    <v-hover v-slot:default="{ hover }">
                        <v-card
                                :elevation="hover ? 12 : 2"
                                :class="{ 'on-hover': hover }"
                                max-width="400"
                        >
                            <v-img
                                    class="white--text align-end"
                                    height="200px"
                                    src="../assets/biurobarys.png"
                            >
                            </v-img>

                            <v-card-subtitle>Strona wizytówka<br>Biuro Rachunkowe Sylwia Baryś</v-card-subtitle>

                            <v-card-text class="text--primary d-flex justify-space-around">
                                <img src="https://image.flaticon.com/icons/svg/1216/1216733.svg" alt="" height="32px">
                                <img src="https://image.flaticon.com/icons/svg/732/732190.svg" alt="" height="32px">
                                <img src="https://image.flaticon.com/icons/svg/919/919828.svg" alt="" height="32px">
                            </v-card-text>

                            <v-card-actions>
                                <v-btn
                                        text
                                        rounded
                                >
                                    Link
                                </v-btn>
                            </v-card-actions>
                        </v-card>
                    </v-hover>
                </div>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
    export default {
        name: "portfolio"
    }
</script>

<style lang="css">
    .v-card {
        transition: opacity .4s ease-in-out;
    }

    .v-card:not(.on-hover) {
        opacity: 0.6;
    }

    .show-btns {
        color: rgba(255, 255, 255, 1) !important;
    }
</style>
