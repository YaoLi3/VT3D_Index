<template>
  <div id="app">
    <header>
      <component  :G_Atlas='G_Atlas' v-bind:is="selected"></component>
    </header>
    <!-- <footer><hr><p>Any page issue or bug resport, please contact: guolidong@genomics.cn; liyao1@genomics.cn; </p><p> Powered by Element.js framework and Echarts.js library.</p></footer> -->
  </div>
</template>

<script>
import Vue from 'vue'
import Element from 'element-ui'
import locale from 'element-ui/lib/locale/lang/en'

Vue.use(Element, { locale })
//import 'element-theme-dark';

import Home from "./Home.vue"

export default {
  data() {
    return {
      G_Atlas:'',
      selected:"Home",
    }
  },
  components:{
     Home,
  },
  methods: {
  },
  mounted(){
  },
}
</script>

<style>
#app {
  font-family: Arial;
  text-align: center;
  margin-top: -8px;
}
hr{
    border:2px solid #ccc;
}
</style>
