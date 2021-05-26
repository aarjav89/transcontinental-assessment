<template>
  <div id="products">
      
      <!-- Top Row -->
           <div class="row" id="row1">
                 <div class="col-lg-9" id="r1col1">
                   <img src="@/assets/images/Row1-1.jpg" alt="" />
                 </div>

                 <div class="col-lg-2" id="r1col2">
                   <img src="@/assets/images/Row1-2.jpg" alt="" />
                 </div>
             </div>
           
           <!-- End of 1st row -->
            
           <!-- 2nd row -->
            
          <div class="row" id="row2">

                <div class="col-lg-6 col-md-9 col-sm-12" >
                  <img src="@/assets/images/Row2-1.jpg" id="img3" alt="">
                </div>
                <div class="col-lg-3 col-md-3 col-sm-12" >
                  <img src="@/assets/images/Row2-2.jpg" id="img4" alt="">
                </div>

                <div class="col-lg-3 col-md-3 col-sm-12" >
                  <img src="@/assets/images/Row2-3.jpg" id="img5" alt="">
                </div>

              
          
           <!-- End of 2nd row  -->

           <!-- Row 3 -->
        
              <div class="col-lg-3 col-md-4" id="row3col1">
                <img src="@/assets/images/Row3-1.jpg" alt="">
                </div>

                <div class="col-lg-3 col-md-4 col-sm-12" id="row3col2">
                <img src="@/assets/images/Row3-2.jpg" alt="">
                </div>

                <div class="col-lg-3 col-md-4 col-sm-12" id="row3col3">
                <img src="@/assets/images/Row3-3.png" alt="">
                </div>

                <div class="col-lg-3 col-md-4 col-sm-12" id="row3col4">
                <img src="@/assets/images/Row3-4.png" alt="">
                </div>


          </div>

           <!-- End of Row 3 -->
     
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

$desktop:1200px;
$laptop: 1024px;
$tablet: 768px;
$phone:572px;

body{
  background: white;
  overflow-x:hidden;
}

#products{
  margin-top:20px;
  width:100%;
  padding:20px;
}

#row1{
  margin-right:20px;
  align-items: center;
}

@media (max-width:1200px){
  #row1{
    display:flex;
    justify-content: space-between;
    flex-wrap: nowrap;
    margin-right:20px;
  }
}

/* Laptop View */
 @media (max-width:1024px){
    #row1{
      display:grid;
      grid-template-columns: repeat(2,minmax(0,1fr)) ;
      margin-right:20px;
    }
    #row2{
      display:grid;
      grid-template-columns: repeat(3,minmax(0,1fr)) ;
      margin-right:20px;
      object-fit:contain;
    }
    


  
}

/* Tablet View */
@media(max-width:972px){
  #row1{
    display:flex;
    justify-content: space-between;
  }
  #row2{
      display:grid;
    grid-template-columns: repeat(2,minmax(0,1fr));
    object-fit: contain;
  }
  #img3{
    max-width: 892px;
  }
  #img4{
    max-width:392px;
  }

}

@media(max-width:802px){
  #row1{
    display:flex;
    justify-content: space-between;
  }
  #row2{
    display:block;
    grid-template-columns: repeat(2,minmax(0,1fr));
    object-fit: contain;
  }
  #r1col2{
    display:none;
  }
  #img3{
    max-width:672px;
  }

}

@media (max-width:572px){
  #row1{
    display:flex;
    justify-content: space-between;
  }
  #row2{
    display:grid;
    grid-template-columns: repeat(1,minmax(0,1fr));

  }

  #img3{
    max-width: 434px;
  }

}


</style>
