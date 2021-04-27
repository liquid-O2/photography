<template>
    <main>
     <div class="hero">
     <div class="text">
     <h1>Lorem ipsum, dolor sit amet consectetur adipisicing elit</h1>
     <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate, dolor odit fuga minus repellendus, cum asperiores, sequi assumenda saepe magni natus in minima aliquid.</p>
     <button class="button-1">View Services</button>
     </div>
    <div class="illustration">
     <img src="../assets/hero1.svg" alt="" srcset="">

    </div>
     </div>
    </main>
</template>

<script>
export default {
    
}
</script>

<style scoped>
main{
    
    pointer-events: none;
    width: 88%;
    margin:auto;
    height: 90vh;
z-index: 1;
}
.hero{
    display: flex;
}
.text{
    padding:10rem 0rem;
    flex: 1 1 40rem;
}
.illustration>img{
    padding-right: 0;
}
.illustration{
    flex: 1 1 40rem;
    padding:3rem 0rem;
    padding-right: 0;
}
.text >h1{
    padding-bottom: 2rem;
   font-size:2.4rem;
}
.text>p{
    font-size:1.2rem;
    line-height: 1.7rem;
}
.text>button{
    margin-top:2rem;
    padding:1rem 1rem;
    font-size:1rem
}
</style>

<style scoped>
@media only screen and (max-width: 1094px) {
  
 .illustration{
     padding:7rem 0rem;
 }
 .hero{
     font-size:0.5rem;
 }
  
 
}
@media only screen and (max-width: 1066px) {
  
.text >h1{
    padding-bottom: 2rem;
   font-size:2rem;
}
.text>p{
    font-size:1rem;
    line-height: 1rem;
}
.text>button{
    margin-top:2rem;
    padding:1rem 1rem;
    font-size:1rem
}
}
@media only screen and (max-width: 850px) {
  
.text >h1{
    padding-bottom: 2rem;
   font-size:1.7rem;
}
.text>p{
    font-size:1rem;
    line-height: 1.5rem;
}
.text>button{
    margin-top:2rem;
    padding:1rem 1rem;
    font-size:1rem
}
.illustration{
    padding:8rem 0rem;
}
}
@media only screen and (max-width: 716px) {
  .hero{
      flex-wrap: wrap;
      text-align: center;
      justify-content: center;
      align-items: center;
  }
.text >h1{
    padding:2rem;
   font-size:2rem;
}
.text>p{
    font-size:1.2rem;
    line-height: 1.8rem;
    font-weight: 300;
}
.text>button{
    margin-top:2rem;
    padding:1rem 1rem  1rem 1rem;
    font-size:1rem
}
.text{
    padding-bottom: 1rem;
    padding-top: 4.5rem;
    margin-bottom: 0rem;
}
.illustration >img{
    width:100%;
    height:100%;
    margin: auto;
    padding-right: 2rem;
}
.illustration{
    padding:2rem;
    width:20rem;
    height:20rem;
   
}
}
.button-1 {
  background-color: none;
  border: 3px solid var(--border-color);
  border-radius: 30px;
  -webkit-transition: all 0.15s ease-in-out;
  transition: all 0.15s ease-in-out;
  color: #1a2930;
  padding: 1.2rem 2rem;
  text-align: center;
  color: var(--text-color);
  pointer-events: all;
}
.button-1:hover {
  box-shadow: 0 0 10px 0 var(--border-color) inset,
    0 0 20px 2px var(--border-color);
  border: 3px solid var(--border-color);
}
.text> h1{
    font-family: 'Source Sans Pro', sans-serif;
    font-weight: 900;
}
.text>p{
     font-family: 'Roboto', sans-serif;
     font-weight: 200;
}
.illustration{
    z-index: 999;
}
</style>