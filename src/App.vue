<template>
  <div id="app">
    <navber></navber>
    <img alt="Vue logo" src="./assets/logo.png">
   
    <buttoncounter></buttoncounter>
    <Calendar></Calendar>
    <slider></slider>

    

  </div>
</template>

<script>
import Vue from "vue";
import { DateRangePickerPlugin } from "@syncfusion/ej2-vue-calendars";

Vue.use(DateRangePickerPlugin);
import buttoncounter from './components/button-counter.vue'
import Calendar from './components/Calendar.vue'
import slider from './components/slider.vue'
import Navber from './components/Navbar.vue'

export default {
  name: 'App',
  components: {
   buttoncounter,Calendar,slider,Navber
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}




@import '../node_modules/@syncfusion/ej2-base/styles/material.css';
@import '../node_modules/@syncfusion/ej2-buttons/styles/material.css';
@import '../node_modules/@syncfusion/ej2-inputs/styles/material.css';
@import '../node_modules/@syncfusion/ej2-popups/styles/material.css';
@import '../node_modules/@syncfusion/ej2-lists/styles/material.css';
@import "../node_modules/@syncfusion/ej2-vue-calendars/styles/material.css";
</style>
