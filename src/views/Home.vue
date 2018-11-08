<template>
  <div class="home">
    
    <MainRed/>
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <SectionRed/>
    <FooterRed/>
  </div>
  
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import MainRed from '@/components/MainRed.vue'
import SectionRed from '@/components/SectionRed.vue'
import FooterRed from '@/components/FooterRed.vue'

export default {
  name: 'home',
  components: {
    HelloWorld,MainRed,SectionRed,FooterRed
  }
}
</script>
