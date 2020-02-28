<template>
  <v-app>
    <Navbar/> 
    <v-content >
      <Date/>
      <Body/>
      <Footer/>
    </v-content>
  </v-app>
</template>

<script>
import Date from './components/Date';
import Navbar from './components/NavBar';
import Body from './views/Home'
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    Date,
    Navbar,
    Body,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>
