<template>
    <v-container>
        <v-row class="Mrow">
            <v-col md="4">
                <h2><span class="Shrort-line"></span>সবচেয়ে</h2>
                    <ul class="tabs" role="tablist">
                        <li>
                            <input type="radio" name="tabs" id="tab1" checked />
                            <label 
                                class="tab1"
                                for="tab1" 
                                role="tab" 
                                aria-selected="true" 
                                aria-controls="panel1" 
                                tabindex="0">শেষ</label>
                            <div id="tab-content1" 
                                class="tab-content" 
                                role="tabpanel" 
                                aria-labelledby="description" 
                                aria-hidden="false">
                            
                                <v-list class="pa-0" color="#F6F6F6">
                                    <v-list-item class="Shobcheyelist">
                                        <p>ওয়ারেন বাফেট এত দিনে ‘স্মার্ট’</p>
                                    </v-list-item>
                                    <v-list-item class="Shobcheyelist">
                                        <p>বৃষ্টিতেও মেলায় ছিল ভিড়</p>
                                    </v-list-item >
                                    <v-list-item class="Shobcheyelist">
                                        <p> অংশগ্রহণ বেড়েছে, অংশীদারত্ব নয়</p>
                                    </v-list-item>
                                    <v-list-item class="Shobcheyelist">
                                        <p>ঋণ খেলাপের দায় আমানতকারীদের ঘাড়ে</p>
                                    </v-list-item>
                                    <v-list-item class="Shobcheyelist">
                                        <p> চট্টগ্রাম বিশ্ববিদ্যালয়-ঘেরা অরণ্য </p>
                                    </v-list-item>
                                    <v-list-item class="listLast">
                                        <p class="red--text">আরও</p>
                                    </v-list-item>
                                </v-list>

                            </div>
                        </li>
                    
                        <li>
                            <input type="radio" name="tabs" id="tab2" />
                            <label for="tab2"
                                role="tab" 
                                aria-selected="false" 
                                aria-controls="panel2" 
                                tabindex="0">আলোচিত</label>
                            <div id="tab-content2" 
                                class="tab-content"
                                role="tabpanel" 
                                aria-labelledby="specification" 
                                aria-hidden="true">
                                <v-list class="pa-0" color="#F6F6F6">
                                    <v-list-item class="Shobcheyelist">
                                        <p>ওয়ারেন বাফেট এত দিনে ‘স্মার্ট’</p>
                                    </v-list-item>
                                    <v-list-item class="Shobcheyelist">
                                        <p>বৃষ্টিতেও মেলায় ছিল ভিড়</p>
                                    </v-list-item >
                                    <v-list-item class="Shobcheyelist">
                                        <p> অংশগ্রহণ বেড়েছে, অংশীদারত্ব নয়</p>
                                    </v-list-item>
                                    <v-list-item class="Shobcheyelist">
                                        <p>ঋণ খেলাপের দায় আমানতকারীদের ঘাড়ে</p>
                                    </v-list-item>
                                    <v-list-item class="Shobcheyelist">
                                        <p> চট্টগ্রাম বিশ্ববিদ্যালয়-ঘেরা অরণ্য </p>
                                    </v-list-item>
                                    <v-list-item class="listLast">
                                        <p class="red--text">আরও</p>
                                    </v-list-item>
                                </v-list>
                            </div>
                        </li>

                        <li>
                            <input type="radio" name="tabs" id="tab3" />
                            <label for="tab3"
                                role="tab" 
                                aria-selected="false" 
                                aria-controls="panel2" 
                                tabindex="0">নির্বাচিত</label>
                            <div id="tab-content2" 
                                class="tab-content"
                                role="tabpanel" 
                                aria-labelledby="specification" 
                                aria-hidden="true">
                                <v-list class="pa-0" color="#F6F6F6">
                                   <v-list-item class="Shobcheyelist">
                                        <p>ওয়ারেন বাফেট এত দিনে ‘স্মার্ট’</p>
                                    </v-list-item>
                                    <v-list-item class="Shobcheyelist">
                                        <p>বৃষ্টিতেও মেলায় ছিল ভিড়</p>
                                    </v-list-item >
                                    <v-list-item class="Shobcheyelist">
                                        <p> অংশগ্রহণ বেড়েছে, অংশীদারত্ব নয়</p>
                                    </v-list-item>
                                    <v-list-item class="Shobcheyelist">
                                        <p>ঋণ খেলাপের দায় আমানতকারীদের ঘাড়ে</p>
                                    </v-list-item>
                                    <v-list-item class="Shobcheyelist">
                                        <p> চট্টগ্রাম বিশ্ববিদ্যালয়-ঘেরা অরণ্য </p>
                                    </v-list-item>
                                    <v-list-item class="listLast">
                                        <p class="red--text">আরও</p>
                                    </v-list-item>
                                </v-list>
                            </div>
                        </li>
                    </ul>
            </v-col>


            <v-col md="8">
                <h2><span class="Shrort-line"></span>বাংলাদেশ</h2>
                <!-- inputfield -->
                <v-row >
                    <v-col class="py-0 px-1" sm="4">
                        <v-overflow-btn
                        class="py-0 px-1"
                        :items="dropdown_font"
                        label="Overflow Btn"
                        outlined
                        target="#dropdown-example"
                        ></v-overflow-btn>
                    </v-col>
                    <v-col class="py-0 px-1" sm="4">

                        <v-overflow-btn
                        class="py-0 px-1"
                        :items="dropdown_font"
                        label="Overflow Btn"
                        outlined
                        target="#dropdown-example"
                        ></v-overflow-btn>
                    </v-col>
                    <v-col class="py-0 px-1" sm="3">

                        <v-overflow-btn
                        class="py-0 px-1"
                        :items="dropdown_font"
                        label="Overflow Btn"
                        outlined
                        target="#dropdown-example"
                        ></v-overflow-btn>
                    </v-col>
                    <v-col class="py-1 px-1" sm="1">
                            <v-btn color="#0091EA" dark large>
                                <v-icon>mdi-magnify</v-icon>
                            </v-btn>
                    </v-col>
                    
                </v-row> 
                <v-row>
                    <v-col md="6">
                        <v-list-item class="white" style="border-top: 1px solid #F0F0ED !important;">
                            <v-list-item-avatar
                            tile
                            size="60"
                            min-width="110px"
                            color="grey"
                            class="ma-1"
                            >
                                <v-img
                                class="white--text align-end"
                                height="auto"
                                width="110px"
                                src="../assets/asset 10.webp"
                                >
                                </v-img>
                            </v-list-item-avatar> 

                            <v-list-item-content class="py-0">
                            <div class=" ml-3">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-col>
                    <v-col md="6">
                        <v-list-item class="white" style="border-top: 1px solid #F0F0ED !important;">
                            <v-list-item-avatar
                            tile
                            size="60"
                            min-width="110px"
                            color="grey"
                            class="ma-1"
                            >
                                <v-img
                                class="white--text align-end"
                                height="auto"
                                width="110px"
                                src="../assets/asset 12.webp"
                                >
                                </v-img>
                            </v-list-item-avatar>               
                            <v-list-item-content class="py-0">
                            <div class=" ml-3">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-col>
                    <v-col md="6">
                       <v-list-item class="white" style="border-top: 1px solid #F0F0ED !important;">
                            <v-list-item-avatar
                            tile
                            size="60"
                            min-width="110px"
                            color="grey"
                            class="ma-1"
                            >
                                <v-img
                                class="white--text align-end"
                                height="auto"
                                width="110px"
                                src="../assets/asset 20.webp"
                                >
                                </v-img>
                            </v-list-item-avatar>               
                            <v-list-item-content class="py-0">
                            <div class=" ml-3">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-col>
                    <v-col md="6">
                        <v-list-item class="white" style="border-top: 1px solid #F0F0ED !important;">
                           <v-list-item-avatar
                            tile
                            size="60"
                            min-width="110px"
                            color="grey"
                            class="ma-1"
                            >
                                <v-img
                                class="white--text align-end"
                                height="auto"
                                width="110px"
                                src="../assets/asset 29.webp"
                                >
                                </v-img>
                            </v-list-item-avatar>               
                            <v-list-item-content class="py-0">
                            <div class=" ml-3">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-col>
                    <v-col md="6">
                        <v-list-item class="white" style="border-top: 1px solid #F0F0ED !important;">
                            <v-list-item-avatar
                            tile
                            size="60"
                            min-width="110px"
                            color="grey"
                            class="ma-1"
                            >
                                <v-img
                                class="white--text align-end"
                                height="auto"
                                width="110px"
                                src="../assets/asset 30.webp"
                                >
                                </v-img>
                            </v-list-item-avatar>               
                            <v-list-item-content class="py-0">
                            <div class=" ml-3">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-col>
                    <v-col md="6">
                        <v-list-item class="white" style="border-top: 1px solid #F0F0ED !important;">
                            <v-list-item-avatar
                            tile
                            size="60"
                            min-width="110px"
                            color="grey"
                            class="ma-1"
                            >
                                <v-img
                                class="white--text align-end"
                                height="auto"
                                width="110px"
                                src="../assets/asset 31.webp"
                                >
                                </v-img>
                            </v-list-item-avatar>               
                            <v-list-item-content class="py-0">
                            <div class=" ml-3">‘খুব দরকার ছিল এ জয়’</div>
                            </v-list-item-content>
                        </v-list-item>
                    </v-col>
                </v-row>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    data:()=>({
        currentTab: 1,
        dropdown_font: ['Arial', 'Calibri', 'Courier', 'Verdana'],
    }),
    methods:{
        changeTab(change){
            this.matchId = change;
            console.log(this.matchId)
            this.selectTab(3);
        },
        selectTab(selectedTab){
            this.currentTab = selectedTab;
        }
    }

}
</script>

<style>
    @media (min-width: 1264px){
        .container {
        max-width: 100%;
        margin-left: 0;
        margin-right: 0; 
        }
        .Mrow{
        margin: 0 58px;
        }
        .tab1{
            margin-left: -24px;
        }
    }
    .tab{
        background-color: #F6F6F6;
    }
    .card{
        background-color: #F6F6F6;
    }

    /* tab css */

        .tabs {
        float: none;
        list-style: none;
        position: relative;
        text-align: left;
        }
        
        .tabs li {
        float: left;
        display: block;
        }
        .tabs input[type="radio"] {
        position: absolute;
        top: 0;
        left: -9999px;
        }
        .tabs label {
        display: block;
        padding: 17px 43.9px;
        border-radius: 2px 2px 0 0;
        font-size: 13px;
        font-weight: normal;
        text-transform: uppercase;
        background: #E7E8E1;
        border-top: 4px solid #999999;
        cursor: pointer;
        position: relative;
        -moz-transition: all 0.2s ease-in-out;
        -o-transition: all 0.2s ease-in-out;
        -webkit-transition: all 0.2s ease-in-out;
        transition: all 0.2s ease-in-out;
        }
        /* .tabs label:hover {
        background: #703688;
        } */
        .tabs .tab-content {
        z-index: 2;
        display: none;
        overflow: hidden;
        width: 100%;
        font-size: 17px;
        line-height: 25px;
        position: absolute;
        top: 53px;
        left: 0;
        background: #F6F6F6;
        }
        .tabs [id^="tab"]:checked + label {
        top: 0;
        padding-top: 17px;
        background: #F6F6F6;
        border-top: 4px solid #424242;
        }
        .tabs [id^="tab"]:checked ~ [id^="tab-content"] {
        display: block;
        }
        .Shobcheyelist{
            border-bottom: 1px solid #CCCCCC;
            background-color: #f6f6f600;
            cursor: pointer;
        }
        .Shobcheyelist:hover{
            background-color: white;
        }
        .listLast{
            display: block;
            position: relative;
            top: 17px;
            text-align: center;
            cursor: pointer;
        }

</style>