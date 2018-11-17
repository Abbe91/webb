<template>
  
  <div id="app">
    

   <HeaderRed/>
    
 
     

     <router-view/>
  </div>
  
</template>




<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
   margin: 3px;
    background-color:hsl(0, 12%, 92%);  
    
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  
  }
}


</style>
