<template>
  <v-container class="background-black">
      <v-row class="Mrow">
          <v-col md="8">
              <h2 class="amber--text">ছবি</h2>
              <v-row class="Background-gray">
                  <v-col class="pt-0 pb-3" md="4">
                    <h3 style="color:#336385;"> <v-icon color="indigo lighten-5">mdi-camera</v-icon> <span class="chobi-titel">এক ঝলক (২৬ ফেব্রুয়ারি, ২০২০)</span> </h3>
                    <vueper-slides fade :touchable="false" :arrows="false" :bullets="false"
                    ref="vueperslides2">
                    <vueper-slide
                    class="slideText"
                    v-for="(slide, i) in slides"
                    :key="i"
                    @click.native="$refs.vueperslides2 && $refs.vueperslides2">
                        <template v-slot:content>
                        <div  :style="'background-color: #33333300'">
                            <p class="white--text chobi-Ptxt">{{ slide.content }}</p>
                        </div>
                        </template>
                    </vueper-slide>
                    </vueper-slides>
                  </v-col>
                  <v-col class="py-0 ml-6" md="6">
                      <vueper-slides
                        @slide="$refs.vueperslides2 && $refs.vueperslides2.goToSlide($event.currentSlide.index, { emit: false })"
                        :slide-ratio="1 / 3"
                        :bullets="false">
                        <vueper-slide
                            v-for="(slide, i) in slides"
                            :key="i"
                            :image="slide.image"
                            />
                        </vueper-slides>
                    </v-col>
              </v-row>
          </v-col>
          <v-col class="background-dark" md="4">
              <h2 class="amber--text">ভিডিও</h2>
              <v-row>
                    <v-card
                        class="mx-auto transparent"
                        max-width="400"
                        outlined
                        style="border-top: 1px solid #333333 !important;"
                        >
                        <v-list-item three-line>
                            <v-list-item-avatar
                            tile
                            size="80"
                            color="grey"
                            ></v-list-item-avatar>              
                            <v-list-item-content>
                            <div class="mb-4 white--text">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-card>
                    <v-card
                        class="mx-auto transparent"
                        max-width="400"
                        outlined
                        style="border-top: 1px solid #333333 !important;"
                        >
                        <v-list-item three-line>
                            <v-list-item-avatar
                            tile
                            size="80"
                            color="grey"
                            ></v-list-item-avatar>              
                            <v-list-item-content>
                            <div class="mb-4 white--text">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-card>
                        <v-card
                        class="mx-auto transparent"
                        max-width="400"
                        outlined
                        style="border-top: 1px solid #333333 !important;"
                        >
                        <v-list-item three-line>
                            <v-list-item-avatar
                            tile
                            size="80"
                            color="grey"
                            ></v-list-item-avatar>              
                            <v-list-item-content>
                            <div class="mb-4 white--text">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-card>
                    <v-card
                        class="mx-auto transparent"
                        max-width="400"
                        outlined
                        style="border-top: 2px solid #333333 !important;"
                    >
                        <v-list-item three-line>
                            <v-list-item-avatar
                            tile
                            size="80"
                            color="grey"
                            ></v-list-item-avatar>              
                            <v-list-item-content>
                            <div class="mb-4 white--text">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-card>
              </v-row>
          </v-col>
      </v-row>
  </v-container>
</template>

<script>
import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'

export default {
    data:()=>({
        // In your component's data.
        slides: [
        {
            title: 'El Teide Volcano, Spain',
            content: 'আঠার বেকী নদীতে জাল ফেলছেন এক জেলে। নন্দনপুর, রূপসা, খুলনা, ২৬ ফেব্রুয়ারি। ছবি: সাদ্দাম হোসেন',
            // You can also provide a URL for the image.
            image: require('@/assets/asset 32.webp')
        },
        {
            title: 'E2 Teide Volcano, Spain',
            content: 'আঠার বেকী নদীতে, রূপসা, খুলনা, ২৬ ফেব্রুয়ারি। ছবি: সাদ্দাম হোসেন',
            // You can also provide a URL for the image.
            image: require('@/assets/asset 33.webp')
        },
        {
            title: 'E3 Teide Volcano, Spain',
            content: 'আঠার ন্দনপুর, রূপসা, খুলনা, ২৬ ফেব্রুয়ারি। ছন',
            // You can also provide a URL for the image.
            image: require('@/assets/asset 34.webp')
        },
        // Other slides.
        ],
    }),
    components: { 
        VueperSlides, 
        VueperSlide 
        },
    methods:{
        ChangeText(text){
            console.log("ok");
        }
    }
}
</script>

<style>
    .background-black{
        background-color: #212121;
    }
    .vueperslides{
        height: 222px;
    }
    .vueperslides__inner{
        width: 433px;
    }
    .vueperslides__parallax-wrapper{
        height: 289px;
        width: 433px;
    }
    .vueperslides__bullet{
        z-index: 0 !important;
    }
    .vueperslides__parallax-wrapper:before, .vueperslides__parallax-wrapper:after{
        box-shadow: none!important;
    }
    .vueperslides__arrow--prev {
        left: -3.5em!important;
        font-size: 10px!important;
    }
    .vueperslides__arrow--next{
        right: -3.5em!important;
        font-size: 10px!important;
    }
    .chobi-Ptxt{
        margin-right: 190px;
        font-size: small;
    }
    .background-dark{
        background-color: #111111 !important;
    }
    .Background-gray{
        background-color: #333333;
        width: 100%;
    }
    .chobi-titel:hover{
        cursor: pointer;
        border-bottom: 3px dashed #336385
    }
    
</style>