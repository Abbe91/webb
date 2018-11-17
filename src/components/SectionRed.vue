<template>
    <section>

        <div class="grid-container">
            <div class="grid-item"><img src="../assets/ts6.jpg" id="expris" alt="swe2"/>
            <p>7,5 USD</p></div>
              <div class="grid-item"><img src="../assets/ts6.jpg" id="expris" alt="swe2"/>
            <p>7,5 USD</p></div>
              <div class="grid-item"><img src="../assets/ts6.jpg" id="expris" alt="swe2"/>
            <p>7,5 USD</p></div>
              <div class="grid-item"><img src="../assets/ts6.jpg" id="expris" alt="swe2"/>
            <p>7,5 USD</p></div>
              <div class="grid-item"><img src="../assets/ts6.jpg" id="expris" alt="swe2"/>
            <p>7,5 USD</p></div>
              <div class="grid-item"><img src="../assets/ts6.jpg" id="expris" alt="swe2"/>
            <p>7,5 USD</p></div>
              <div class="grid-item"><img src="../assets/ts6.jpg" id="expris" alt="swe2"/>
            <p>7,5 USD</p></div>
              <div class="grid-item"><img src="../assets/ts6.jpg" id="expris" alt="swe2"/>
            <p>7,5 USD</p></div>
             
            
        </div>

    </section>
</template>

<script>
export default {
    name:'sectionred',
    components:{

    }
}
</script>

<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto;
  
  padding: 10px;


}
.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border-radius: 12px;
  padding: 30px;
  font-size: 30px;
  text-align: center;
      
  background-color: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  margin-bottom: 25px;
  margin-right: 50px;
   margin-left: 50px;

}
#expris{
  
    border-radius: 20px;
    width: 120px;
    height: 120;
    background: #999;
    border-radius: 12px;
    border-radius: 80px;

 
}
p{
    font-size: 100%
}
</style>



