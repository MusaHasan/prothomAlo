<template>
  <v-container>
      <v-row class="Mrow">
          <v-col md="8">
              <v-row>
                  <v-col md="4">
                      
                      <h3> <v-icon>mdi-camera</v-icon> এক ঝলক (২৬ ফেব্রুয়ারি, ২০২০)</h3>
                      <vueper-slides fade :touchable="false" :arrows="false" :bullets="false"
                        ref="vueperslides2">
                        <vueper-slide
                        class="slideText"
                        v-for="(slide, i) in slides"
                        :key="i"
                        @click.native="$refs.vueperslides2 && $refs.vueperslides2">
                            <template v-slot:content>
                            <div  :style="'background-color: #FFFFFF'">
                                <p>{{ slide.content }}</p>
                            </div>
                            </template>
                        </vueper-slide>
                        </vueper-slides>
                  </v-col>
                  <v-col md="8">
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
          <v-col md="4"></v-col>
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
    .vueperslides__bullet{
        z-index: 0 !important;
    }
    .vueperslides__parallax-wrapper:before, .vueperslides__parallax-wrapper:after{
        box-shadow: none!important;
    }
    .slideText .vueperslides__arrows{
        color: #000!important;
    }
</style>