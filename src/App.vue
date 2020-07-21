<template>
  <v-app>
    <navbar/>
    <v-main>
      <Main/>
    </v-main>
  </v-app>
</template>

<script>
import Main from './components/Main';
import Navbar from "./components/Navbar";

export default {
  name: 'App',

  components: {
    Main,
    Navbar
  },

  data: () => ({
    //
  }),
};
</script>
