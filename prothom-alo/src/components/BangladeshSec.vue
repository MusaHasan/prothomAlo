<template>
    <v-container>
        <v-row class="Mrow">
            <v-col md="4">
                <h2>সবচেয়ে</h2>
                <!-- <v-card >
                <v-tabs background-color="#E7E8E1" >
                    <v-tab class="tab" @click="selectTab(1)" ><p>শেষ</p></v-tab>
                    <v-tab class="tab" @click="selectTab(2)" ><p>আলোচিত</p></v-tab>
                    <v-tab class="tab" @click="selectTab(3)" ><p>নির্বাচিত</p></v-tab>
                </v-tabs>
                <v-sheet
                id="scrolling-techniques-3"
                >
                <v-container class="card">
                    <v-row v-if="currentTab==1" class="bg-grey-light p-8">
                        <h3>section 1 comming soon..</h3>
                    </v-row>

                    <v-row v-if="currentTab==2"   class="bg-grey-light p-8">
                            <h3>section 2 comming soon..</h3>
                    </v-row>

                    <v-row v-if="currentTab==3" class="bg-grey-light p-8">
                        <h3>section 3comming soon..</h3>
                    </v-row>
                    
                </v-container>
                </v-sheet>
                </v-card> -->
                    <ul class="tabs" role="tablist">
                        <li>
                            <input type="radio" name="tabs" id="tab1" checked />
                            <label 
                                class="tab1"
                                for="tab1" 
                                role="tab" 
                                aria-selected="true" 
                                aria-controls="panel1" 
                                tabindex="0">Description</label>
                            <div id="tab-content1" 
                                class="tab-content" 
                                role="tabpanel" 
                                aria-labelledby="description" 
                                aria-hidden="false">
                            
                                <v-card
                                    class="mx-auto"
                                    max-width="344"
                                    outlined
                                >
                                    <v-list-item three-line>
                                    <v-list-item-content>
                                        <v-list-item-title class="headline mb-1">Headline 5</v-list-item-title>
                                    </v-list-item-content>
                                    </v-list-item>
                                </v-card>

                            </div>
                        </li>
                    
                        <li>
                            <input type="radio" name="tabs" id="tab2" />
                            <label for="tab2"
                                role="tab" 
                                aria-selected="false" 
                                aria-controls="panel2" 
                                tabindex="0">Specification</label>
                            <div id="tab-content2" 
                                class="tab-content"
                                role="tabpanel" 
                                aria-labelledby="specification" 
                                aria-hidden="true">
                            <p>"Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla?</p>
                            </div>
                        </li>

                        <li>
                            <input type="radio" name="tabs" id="tab3" />
                            <label for="tab3"
                                role="tab" 
                                aria-selected="false" 
                                aria-controls="panel2" 
                                tabindex="0">Specification</label>
                            <div id="tab-content2" 
                                class="tab-content"
                                role="tabpanel" 
                                aria-labelledby="specification" 
                                aria-hidden="true">
                            <p>"Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla?</p>
                            </div>
                        </li>
                    </ul>
                
            </v-col>


            <v-col md="8">
                <h2>বাংলাদেশ</h2>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    data:()=>({
        currentTab: 1,
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
        padding: 17px 24px;
        border-radius: 2px 2px 0 0;
        font-size: 14px;
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
        padding: 25px;
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

</style>