<template>
  <div class="home">
    <Section1/>
    <Bangladesh/>
    <Khela/>
    <Binodon/>
    <Motamot/>
    <ChobiVideo/>
    <Adhuna/>
    <Antorjatik/>
    <Arthoniti/>
    <AppStor/>
  </div>
</template>

<script>
// @ is an alias to /src
import Section1 from '@/components/Section1.vue'
import Bangladesh from '@/components/BangladeshSec.vue'
import Khela from '@/components/KhelaSec.vue'
import Binodon from '@/components/binodonSec.vue'
import Motamot from '@/components/MotamotSec.vue'
import ChobiVideo from '@/components/VideoSec.vue'
import Adhuna from '@/components/AdhunaSec.vue'
import Antorjatik from '@/components/AntorjatikSec.vue'
import Arthoniti from '@/components/ArthonitiSec.vue'
import AppStor from '@/components/AppStorSec.vue'

export default {
  name: 'Home',
  components: {
    Section1,
    Bangladesh,
    Khela,
    Binodon,
    Motamot,
    ChobiVideo,
    Adhuna,
    Antorjatik,
    Arthoniti,
    AppStor
  }
}
</script>
