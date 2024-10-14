<template>
  <div>
    <TopNavBar />
  </div>
  <div class="Header">
    <div id='rssBlock'>
  <p class="cnnContents">
      <span class="marqueeStyle">Portfolio   Portfolio   Portfolio   Portfolio   Portfolio   Portfolio  Portfolio   Portfolio   Portfolio   Portfolio   Portfolio   Portfolio</span>
        <span class="marqueeStyle2">Portfolio   Portfolio   Portfolio   Portfolio   Portfolio   Portfolio  Portfolio   Portfolio   Portfolio   Portfolio   Portfolio   Portfolio</span>
    </p>
    </div>
  </div>
  <div class="About">
    <AboutVue />
    </div>
  <div class="Contract">
    <Contract />
    </div>
  <RouterView />
</template>
<script>
import { RouterView } from 'vue-router';
import AboutVue from './views/About.vue';
import TopNavBar from './views/TopNavBar.vue';
import Contract from './views/Contract.vue'

export default {
components: {
  TopNavBar,
  AboutVue,
  Contract,
}
}
</script>
<style>
*{
  
}
/* Header */
#rssBlock{
  left:0px;
  height: 80px;
  background: #FFFFFF;
  position: absolute;
  width:100%;
  overflow: hidden;
}

/*remove p*/
.cnnContents {
  width:100%;
  padding-top: 20px;
  margin:0 auto;
  font-size: 30px;
  white-space: nowrap;
  text-transform: uppercase;
  font-family: 'Museo';
  font-weight: 300;
}

.marqueeStyle {
  display:inline-block;
  padding-right: 15%;
  /* Apply animation to this element */
  -webkit-animation: scrolling-left1 20s linear infinite;
  animation: scrolling-left1 20s linear infinite;
}

.marqueeStyle2 {
  display:inline-block;
  padding-right: 15%;
  /* Apply animation to this element */
  -webkit-animation: scrolling-left2 20s linear infinite;
  animation: scrolling-left2 20s linear infinite;
  animation-delay: 0s;
}
/* scrolling-left is continuous/repeatly text */
@keyframes scrolling-left1 {
    0% {transform: translateX(100%);
        -webkit-transform: translateX(100%);}
      100% {transform: translateX(-100%);
          -webkit-transform: translateX(-100%);}
}
@keyframes scrolling-left2 {
    0% {transform: translateX(0%);
        -webkit-transform: translateX(0%);}
      100% {transform: translateX(-200%);
          -webkit-transform: translateX(-200%);}
}

@-webkit-keyframes scrolling-left1 {
    0% {-webkit-transform: translateX(100%);}
      100% {-webkit-transform: translateX(-100%);}
}
@-webkit-keyframes scrolling-left2 {
    0% {-webkit-transform: translateX(0%);}
      100% {-webkit-transform: translateX(-200%);}
}
/* About */
</style>
