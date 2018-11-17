<template>
  
  <div class="home">
      
   
    <HeaderRed/>
   
    <MainRed/>
 
    <HelloWorld/>
    <SectionRed/>
    <FooterRed/>
  </div>
  
</template>

<script>
// @ is an alias to /src
import HeaderRed from '@/components/HeaderRed.vue'
import HelloWorld from '@/components/HelloWorld.vue'
import MainRed from '@/components/MainRed.vue'
import SectionRed from '@/components/SectionRed.vue'
import FooterRed from '@/components/FooterRed.vue'


export default {
  name: 'home',
  components: {
    HelloWorld,MainRed,SectionRed,FooterRed,HeaderRed
  }
}

</script>
<style>
.home {
  display:grid;
  height:130vw;
  grid-template-rows:10vh minmax(20vh,30vh) minmax(5vh,20vh);
  grid-gap:10px;
  grid-template-areas:
  'hd hd hd'
  'mn mn mn'
  '.  .  . '
  '.  .  . '
  'sc sc sc'
  'ft ft ft'
}
header{
  grid-area: hd;

}
nav{
  grid-area: nv;
}
main{
  grid-area: mn;
}
section{
  grid-area: sc;
}
footer{
  grid-area: ft;
}

</style>

