<template>
  <v-container>
    <v-row class="white">
      <v-col cols="12" class="mt-12 pt-10 px-0 text outlined">
        <p>
            <span> <v-icon class="body-1 mb-1">mdi-map-marker</v-icon> ঢাকা</span> 
            <span> <v-icon class="body-1 mb-1">mdi-calendar-month</v-icon> মঙ্গলবার, ২৫ ফেব্রুয়ারি ২০২০, ১২ ফাল্গুন ১৪২৬, ৩০ জমাদিউস সানি ১৪৪১ </span> 
            <span><v-icon class="body-1 mb-1">mdi-clock-outline</v-icon> আপডেট ১০ মিনিট আগে</span> 
          </p>
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
  }
  .text{
    font-size: 0.775rem !important;
    font-weight: 400;
    letter-spacing: 0.0178571429em !important;
    line-height: 1.25rem;
    font-family: "Roboto", sans-serif !important;
    margin-left: 63px;
  }
  .text span{
    margin-right: 20px; 
  }
  

</style>
