<template>
  <v-container>
    <v-row class="white Mrow">
      <v-col md="2">
          <v-img class="logo" src="../assets/pLogo.png"></v-img>
      </v-col>
      <v-col md="5">

      </v-col>
      <v-col md="5">
        <v-row>
          <p class="text">মোবাইল অ্যাপস ডাউনলোড করুন</p>
          <v-img class="icon1" src="../assets/Apple-aps-icon.jpg"></v-img>
          <v-img class="icon2" src="../assets/googlePlayIc.png"></v-img>
      
        </v-row>
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
      width: 70%;
      height: fit-content;
    }
    .text{
      font-size: 11px; 
      margin-top: 12px;
      position: relative;
      right: -55px;
    }
    .icon1{
      width: 20%;
      height: fit-content;
      margin: -8px 54px;
      position: relative;
      left: 31px;
      cursor: pointer;
    }
    .icon2{
      width: 20%;
      height: fit-content;
      cursor: pointer;
    }


</style>
