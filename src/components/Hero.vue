<template>
    <v-parallax
            dark
            src="../assets/hero.jpg"
            height="600">
        <v-row justify="center"
               align="center">
            <v-col
                    cols="8">
                <h2>Daniel Sobieraj</h2>
                <h2 class="navbar-title">Junior
                    <span class="typed-text">{{ typeValue }} </span>
                    <span class="cursor" :class="{'typing': typeStatus}">&nbsp;</span>
                </h2>
            </v-col>

        </v-row>
    </v-parallax>
</template>

<script>
    export default {
        name: 'Hero',
        data() {
            return {
                typeValue: '',
                typeStatus: true,
                typeArray: ['Front-End Developer', 'Web Developer'],
                typingSpeed: 100,
                erasingSpeed: 50,
                newTextDelay: 2000,
                typeArrayIndex: 0,
                charIndex: 0,
            }
        },
        methods: {
            typeText() {
                if (this.charIndex < this.typeArray[this.typeArrayIndex].length) {
                    if (!this.typeStatus)
                        this.typeStatus = true;
                    this.typeValue += this.typeArray[this.typeArrayIndex].charAt(this.charIndex);
                    this.charIndex += 1;
                    setTimeout(this.typeText, this.typingSpeed);
                } else {
                    this.typeStatus = false;
                    setTimeout(this.eraseText, this.new);
                }

            },
            eraseText() {
                if (this.charIndex > 0) {
                    if (!this.typeStatus)
                        this.typeStatus = true;

                    this.typeValue = this.typeArray[this.typeArrayIndex].substring(0, this.charIndex - 1);
                    this.charIndex -= 1;
                    setTimeout(this.eraseText, this.erasingSpeed);
                } else {
                    this.typeStatus = false;
                    this.typeArrayIndex += 1;
                    if (this.typeArrayIndex >= this.typeArray.length)
                        this.typeArrayIndex = 0;

                    setTimeout(this.typeText, this.typingSpeed + 1000);
                }

            }
        },
        created() {
            setTimeout(this.typeText, this.newTextDelay + 200)
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

    span.typed-text {
        color: #41B883;
    }

    span.cursor {
        display: inline-block;
        margin-left: 4px;
        width: 4px;
        background-color: white;
        animation: cursorBlink 1s infinite;
    }

    span.cursor.typing {
        animation: none;
    }

    @keyframes cursorBlink {
        49% {
            background-color: white;
        }
        50% {
            background-color: transparent;
        }
        99% {
            background-color: transparent;
        }

    }
</style>
