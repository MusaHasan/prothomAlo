<template>
    <v-app-bar
        fixed
        color="white"
        elevate-on-scroll
        style="border-bottom: 1px solid #CCCCCC !important;"
    >
        <v-container   
        class="navbar">
            <img class="logo" src="../assets/pLogo.png" alt="">
            
            <v-spacer></v-spacer>

            <v-btn class="navItem" v-for="button in buttons" :key="button.name">
                {{button.name}}
            </v-btn>

            <v-btn class="navItem">
                <v-app-bar-nav-icon></v-app-bar-nav-icon>
                সব
            </v-btn>

            <div style="width: 1px;height: 20px; margin:auto; background-color:black;"></div>

            <v-btn class="navItem redtext">
                English
            </v-btn>

            <v-btn class="navItem navIcn" v-for="icon in icons" :key="icon.ic">
                <v-icon class="navIcn">{{icon.ic}}</v-icon>
            </v-btn>
        </v-container>
    </v-app-bar>
</template>

<script>
export default {
    data:()=>({
        buttons:[
            { id: 1, name: "বাংলাদেশ"}, { id:2, name:"আন্তর্জাতিক"},{ id:3, name:"অর্থনীতি"}, { id:3, name:"মতামত"},{ id:4, name:"খেলা"},
            { id:5, name: "বিনোদন"}, { id:6, name:"উত্তর আমেরিকা"}, {id:7, name:"জীবনযাপন"},{ id:8, name:"ভিডিও"}
        ],
        icons:[
            {id:1, ic:"mdi-account-circle"}, { id:2, ic:"mdi-magnify"}, {id:3, ic:"mdi-thumb-up"}
        ]
    })

}
</script>

<style>
    @media (min-width: 1264px){
        .v-toolbar__content, .v-toolbar__extension {
            padding: 4px 64px !important;
        }
    }
.logo{
    width: 16%;
    height: fit-content;
}
.navbar{
    width: 100%;
    display: flex;
    margin-left: 51px;
    margin-bottom: -12px;
    padding: 0px;
}
.navItem{
    box-shadow: none !important;
    background-color: #f0f8ff00 !important;
    padding: 0 5.4px !important;
    min-width: 31px !important;
    height: 60px !important;
    font-size: 13px !important;
    margin-top: -9px;
}
.navIcn{
    border-radius: 20%;
}
.redtext{
    color: #D94141 !important;
    font-size: 10px !important;
}
</style>