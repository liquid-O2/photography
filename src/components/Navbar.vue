<template>
    <header>
        
        <nav>
          <ul class="navbar">
            <li class= "navbar_items item1" id="logo">Logo</li>
             
             <li class= "navbar_items item3">Services</li>
             <li class= "navbar_items item4">
                 <div @click="toggleIcon">
                     <span v-if="theme === 'dark'">Dark Mode</span>
                     <span v-else >Light Mode</span>
                 
                 </div></li>
          </ul>
        </nav>
    
    
    
    </header>
</template>

<script>
export default {
    props:[ 'theme' ],
    methods:{
        toggleIcon(){
            this.$emit('toggleSelf')
        }
    }
}
</script>

<style>
header{
    top: 0;
    width: 90%;
    margin: auto;
    padding: 1rem 0rem;
    height: 10vh;
    
    
}
.navbar{
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}
li{
    list-style: none;
    padding: 0 1rem;
}

.navbar-items{
   flex:1 1 40rem;
   
   align-items: center;
}
.item2,.item3,.item4{
    padding-top: 0.3rem;
}
.item1{
flex:2 1 30rem;
}
#logo{
    font-family: 'Roboto Condensed', sans-serif;
}

@media only screen and (max-width: 968px) {
  
 #logo{
     width: 100%;
     flex:3 1 60rem;
     text-align: center;
     padding-bottom: 1rem;
  
     
 }
  .navbar-items{
      flex:1 1 4rem;
      
      
  }

}


</style>
<style scoped>

*{
    font-size:1.2rem;
     font-weight: 400;
}

#logo{
    font-size:2rem;
    font-weight: bold;
    text-transform: uppercase;
}
@media only screen and (max-width: 478px) {
  
 
  *{
      font-size: 1.2rem;
  }
  .navbar-items{
      justify-content: center;
     
  }
 
}

@media only screen and (max-width: 390px) {
  
 
 *{
     font-size: 1rem;
 }
}
 
 .navbar{
     padding-top: 1.3rem;
 }
*{
    font-family: 'Source Sans Pro', sans-serif;
}

</style>