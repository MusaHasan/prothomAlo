<template>
  <v-container>
    <v-row class="white Mrow">
      <v-col>
        <v-img class="logo" src="../assets/pLogo.png"></v-img>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {

    data: () => ({
    }),
  }
</script>
<style scoped>
  @media (min-width: 1264px){
    .container {
      max-width: 100%;
      margin-left: 0;
      margin-right: 0; 
    }
    .Mrow{
      margin: 0 58px;
    }
  }
  .logo{
    width: 16%;
    height: fit-content;
}

</style>
