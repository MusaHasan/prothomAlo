<template>
    <v-container>
        <v-row class="Mrow">
            <v-col md="8">
                <H2><span class="Shrort-line"> </span> অধুনা</H2>
                <v-row>
                    <v-col md="4">
                        <v-card
                        class="mx-auto"
                        max-width="100%"
                        :elevation="0"
                        tile
                        color="#F0F0ED"
                        >
                            <v-img
                                class="white--text align-end"
                                height="200px"
                                src="../assets/asset 50.webp"
                            >
                            </v-img>

                            <h4 class="pa-4 pb-0">দলীয় প্রতিদ্বন্দ্বীদের তোপের মুখে স্যান্ডার্স</h4>
                            <v-card-text class="text--primary pt-0">
                                <div>বাছাই পর্বের প্রথম তিন নির্বাচনে সবচেয়ে বেশি ভোট পেয়ে বার্নি স্যান্ডার্স এই...</div>
                            </v-card-text>
                        </v-card>
                    </v-col>
 
                    <v-col md="4">
                        <v-card
                        class="mx-auto"
                        max-width="100%"
                        :elevation="0"
                        tile
                        color="#F0F0ED"
                        >
                            <v-img
                                class="white--text align-end"
                                height="200px"
                                src="../assets/asset 51.webp"
                            >
                            </v-img>

                            <h4 class="pa-4 pb-0">দলীয় প্রতিদ্বন্দ্বীদের তোপের মুখে স্যান্ডার্স</h4>
                            <v-card-text class="text--primary pt-0">
                                <div>বাছাই পর্বের প্রথম তিন নির্বাচনে সবচেয়ে বেশি ভোট পেয়ে বার্নি স্যান্ডার্স এই...</div>
                            </v-card-text>
                        </v-card>
                    </v-col>
 
                    <v-col md="4">
                        <v-card
                        class="mx-auto"
                        max-width="100%"
                        :elevation="0"
                        tile
                        color="#F0F0ED"
                        >
                        <v-img
                            class="white--text align-end"
                            height="200px"
                            src="../assets/asset 52.webp"
                        >
                        </v-img>

                        <h4 class="pa-4 pb-0">দলীয় প্রতিদ্বন্দ্বীদের তোপের মুখে স্যান্ডার্স</h4>
                        <v-card-text class="text--primary pt-0">
                            <div>বাছাই পর্বের প্রথম তিন নির্বাচনে সবচেয়ে বেশি ভোট পেয়ে বার্নি স্যান্ডার্স এই...</div>
                        </v-card-text>
                    </v-card>
                    </v-col>
                </v-row>
            </v-col>
            <v-col md="4">
                <h2><span class="Shrort-line"></span> ছবির গল্প</h2>
                <v-row class="mt-3">
                    <v-img class="mb-1" src="https://picsum.photos/510/300?random" width="100%" aspect-ratio="1.7"></v-img>
                    <H3>ফুলকপির পাশাপাশি চাষ হচ্ছে ব্রকলিও</H3>
                </v-row>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {

}
</script>

<style>
.Shrort-line{
    padding: 0px 3px;
    margin-right: 16px;
    background-color: #D84315;
}
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
@media only screen and (min-width: 1380px) {
  .home{
    margin: 0 5%!important;

  }
}
</style>