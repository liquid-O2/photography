<template>
 <div id="sc1">
<Navbar :theme="theme" @toggleSelf="tggle" />
<Hero/>
</div>
<div id="sc2">
<Services />
</div>
</template>

<script>
import Navbar from "./components/Navbar.vue" 
import Hero from "./components/Hero.vue" 
import Services from "./components/Services"
export default {
  name: 'App',
  data(){
    return{
     theme:''
    }
    
  },
  components:{
     Navbar, Hero, Services
  },
  methods:{
    tggle(){
      if(this.theme === 'dark'){
        this.theme=''
      }
      else{
        this.theme = 'dark'
      }
      document.documentElement.setAttribute("data-theme", this.theme)
    }
  }
   
  
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@400;900&display=swap');
:root {
  /* Variables for default theme (light-mode) */
  --background-color: #f5f5f5;
  --text-color: black;
  --border-color: #1a2930;
}
body {
  background-color: var(--background-color);
  color: var(--text-color);
  font-family: 'Roboto', sans-serif;
}

[data-theme="dark"] {
  /* Variables for dark mode */
  --background-color: black;
  --text-color: #c5c1c0;
  --border-color: #d1d0d0;
}
button{
  background:none;
  cursor: pointer;
}
#sc1{
 position:relative;
overflow: initial;
}
#sc2{
  overflow: hidden;
}
</style>
