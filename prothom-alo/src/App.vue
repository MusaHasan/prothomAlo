<template>
  <v-app>
    <Navbar/> 
    <v-content >
      <Date/>
      <Body/>
    </v-content>
  </v-app>
</template>

<script>
import Date from './components/Date';
import Navbar from './components/NavBar';
import Body from './views/Home'

export default {
  name: 'App',

  components: {
    Date,
    Navbar,
    Body
  },

  data: () => ({
    //
  }),
};
</script>
