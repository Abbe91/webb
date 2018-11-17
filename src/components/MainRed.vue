<template>
    <main>
   
  <input type="text" id="myInput" onkeyup="myFunction()" placeholder="Search for names.." title="Type in a name">
      <div class="bildspel">
                <img  class="logo" src="../assets/girl.jpg" id="bildspel1" alt="swe2"/>
               <h1 class="city">ABBE</h1>  
               <!-- <img  class="logo" src="../assets/sweatshirts.jpg" id="bildspel1" alt="Bild på logo"/>
               <h1 class="city">ABBE</h1>               
               <img  class="logo" src="../assets/Multicolored.jpg" id="bildspel1" alt="swe3"/>
               <h1 class="city">ABBE</h1> -->
       
                
               <br/>     
  
               <div id="caption"> caption dor slide1 </div>
             
           
               
               <button type="button" class="btn btn-danger" v-on:click="changeImage(-1)">Nästa bilden</button>
               <button type="button" class="btn btn-success" v-on:click="changeImage(+1)">Före bilden</button>
      </div>
        
    </main>

</template>

<script>

   var images = ["/img/sweatshirts.1390a1c8.jpg","/img/girl.2c6e3292.jpg","/img/Multicolored.09e3a5ea.jpg"];
    var caption = ["sweden1", "sweden2","sweden3"];

    var imageNumber=0;
    var imageLength= images.length - 1;
export default {
    name:'ManiRed',
    
    components:{

    },

    created: function(){
        
      
    },
 
    methods:{
        
        changeImage(x){
        console.log('asdd');
        imageNumber += x;
        //Om du har nått slutet av arrayen, börja om
        if (imageNumber> imageLength){
            imageNumber =0;
        }
        if (imageNumber <0){
            imageNumber=imageLength;
        }
        document.getElementById("bildspel1").src= images[imageNumber];
        document.getElementById("caption").innerHTML = caption[imageNumber];
        

        return false;
    }
    
}
}

 
        




</script>

<style>

#myInput {
  background-image: url('/css/searchicon.png');
  background-position: 10px 10px;
  background-repeat: no-repeat;
  width: 100%;
  font-size: 16px;
  padding: 12px 20px 12px 40px;
  border: 1px solid #ddd;
  margin-bottom: 12px;
}

.logo{
    background-color: white;
  box-shadow: 0 20px 40px 0 rgba(0, 0, 0, 0.2), 0 30px 90px 0 rgba(0, 0, 0, 0.19);
  margin-bottom: 25px;
  
}


img {
    vertical-align: middle;
    
    
}
button{
    color:blue;
}
.auto{
    display: none;
}
* {
  box-sizing: border-box;
}

#myInput {
  background-image: url('/css/searchicon.png');
  background-position: 10px 10px;
  background-repeat: no-repeat;
  width: 100%;
  font-size: 16px;
  padding: 12px 20px 12px 40px;
  border: 1px solid #ddd;
  margin-bottom: 12px;
}

#myTable {
  border-collapse: collapse;
  width: 100%;
  border: 1px solid #ddd;
  font-size: 18px;
}

#myTable th, #myTable td {
  text-align: left;
  padding: 12px;
}

#myTable tr {
  border-bottom: 1px solid #ddd;
}

#myTable tr.header, #myTable tr:hover {
  background-color: #f1f1f1;
}
</style>


