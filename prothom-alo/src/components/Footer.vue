<template>
  <v-container class="bgBlack">
      <v-row class="Mrow bgBlack">
              <v-col md="2" >
                  <v-col class="pa-1" v-for="(list,i) in lists1" :key="i">
                      {{list.name}}
                  </v-col>
                </v-col >
                <v-col md="2" >
                  <v-col class="pa-1" v-for="(list,i) in lists2" :key="i">
                      {{list.name}}
                  </v-col>
                </v-col >
                <v-col md="2" >
                  <v-col class="pa-1" v-for="(list,i) in lists3" :key="i">
                      {{list.name}}
                  </v-col>
                </v-col >
                <v-col md="2" >
                  <v-col class="pa-1" v-for="(list,i) in lists4" :key="i">
                      {{list.name}}
                  </v-col>
                </v-col >
                <v-col md="2" >
                  <v-col class="pa-1" v-for="(list,i) in lists5" :key="i">
                      {{list.name}}
                  </v-col>
                </v-col >
                <v-col md="2" >
                  <v-col class="pa-1" v-for="(list,i) in lists6" :key="i">
                      <p> <v-icon color="blue darken-2">{{list.ic}}</v-icon> {{list.name}}</p>
                      
                  </v-col>
              </v-col >
      </v-row>
      <v-row class="Mrow">
          <v-col md="8">
              <v-row>
                  <v-col md="1" class="caption">বিজ্ঞাপন</v-col>
                  <v-col md="1" class="caption">সার্কুলেশন</v-col>
                  <v-col md="2" class="caption">পবিত্র হজ</v-col>
                  <v-col class=" americaTxt caption">উত্তর আমেরিকা</v-col>
              </v-row>
              <v-row>
                <v-col md="2" class="caption"><img src="../assets/asset 1.png" alt=""> <span class="companyLogo">২২২২১</span> </v-col>
                <v-col md="2" class="caption"><img src="../assets/asset 2.png" alt=""> <span class="companyLogo">ট্রাস্ট</span> </v-col>
                <v-col md="2" class="caption"><img src="../assets/asset 3.png" alt=""> <span class="companyLogo">প্রতিচিন্তা</span> </v-col>
                <v-col md="2" class="caption"><img src="../assets/asset 4.png" alt=""> <span class="companyLogo">কিশোর আলো</span>  </v-col>
                <v-col md="2" class="caption"><img src="../assets/asset 5b.png" alt=""></v-col>
                <v-col md="2" class="caption"><img src="../assets/asset 5.png" alt=""> <span class="companyLogo">abc রেডিও</span>  </v-col>
              </v-row>
              <v-row>
                  <v-col md="10"></v-col>
                  <v-col><img src="../assets/asset 6.png" alt=""></v-col>
              </v-row>
              <v-row>
                  <v-col class="caption"><img src="../assets/asset 7.png" alt=""><span class="companyLogo">প্রথমা</span></v-col>
              </v-row>
          </v-col>
          <v-col class="overline" md="4" >
              <p><span class="font-italic body-2 font-weight-medium">Prothom Alo</span> is the highest circulated and most read newspaper in Bangladesh. 
                  The online portal of <span class="font-italic body-2 font-weight-medium">Prothom Alo</span> is the most visited Bangladeshi and Bengali website in the world.</p>
                <p>
                    Privacy Policy | Terms of Use
                </p>
          </v-col>
      </v-row>
      <v-row class="container txt px-0">
        <v-row class="Mrow ">
          <p>© স্বত্ব প্রথম আলো ১৯৯৮ - ২০২০</p>
          <p>সম্পাদক ও প্রকাশক: মতিউর রহমান</p>
          <p>প্রগতি ইনস্যুরেন্স ভবন, ২০-২১ কারওয়ান বাজার , ঢাকা ১২১৫</p>
          <p>ফোন: ৮১৮০০৭৮-৮১, ফ্যাক্স: ৫৫০১২২০০, ৫৫০১২২১১ ইমেইল: info@prothomalo.com</p>
        </v-row>
      </v-row>
      
  </v-container>
</template>

<script>
export default {
    data:()=>({
        lists1:[
            {name: "প্রচ্ছদ"},
            {name: "মতামত"},
            {name: "অন্য আলো"}
        ],
        lists2:[
            {name: "বাংলাদেশ"},
            {name: "বিনোদন"},
            {name: "পাঁচমিশালি"}
        ],
        lists3:[
            {name: "আন্তর্জাতিক"},
            {name: "ফিচার"},
            {name: "আমরা"}
        ],
        lists4:[
            {name: "অর্থনীতি"},
            {name: "জীবনযাপন"},
             {name: "শিক্ষাি"}
        ],
        lists5:[
            {name: "খেলা"},
            {name: "বিজ্ঞান ও প্রযুক্তি"}
        ],
        lists6:[
            {name: "ছবি", ic:"mdi-camera"},
            {name: "ভিডিওি", ic:"mdi-video"},
            {name: "আর্কাইভ", ic:"mdi-file-cad"}
        ]
    })

}
</script>

<style>
     @media (min-width: 1264px){
    .container {
      max-width: 100%;
      margin-left: 0;
      margin-right: 0; 
      padding-left: 0!important;
      padding-right: 0!important;
    }
    .Mrow{
      margin: 0 58px;
      
    }
    .bgBlack{
        background-color: #282828;
        color: #C2CCCC;
        border-bottom: 1px solid;
    }
    .txt{
        background-color: #181818;
        color: #999999;
    }
    .txt p{
        width: 100%;
    }
    .companyLogo{
        position: relative;
        top: -8px;
    }
    .americaTxt{
        position: relative;
        left: -60px;
    }
  }
</style>