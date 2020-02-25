<template>
  <div class="home">
    <Section1/>
    <Bangladesh/>
  </div>
</template>

<script>
// @ is an alias to /src
import Section1 from '@/components/Section1.vue'
import Bangladesh from '@/components/BangladeshSec.vue'

export default {
  name: 'Home',
  components: {
    Section1,
    Bangladesh
  }
}
</script>
