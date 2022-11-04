<template>
  <div class="home">
    Hello
  </div>
  <div class = "threeBox">
    <div class = "box1">
    </div>
    <div class = "box2">
    </div>
    <div class = "box3">
    </div>
  </div>
</template>

<style scoped>
.home{
  position: absolute;
  background-color:#D9D9D9;
  top: 5%; right: 4.2%;
  width: 900px;
  height: 500px;
  border-radius: 4px;
  transition: transform .2s;

  }
  .box1{
    position: absolute;
    background-color:#D9D9D9;
    top: 70%; right: 58.4%;
    width: 250px;
    height: 230px;
    border-radius: 4px;
    transition: transform .2s;
  }
  .box2{
    position: absolute;
    background-color:#D9D9D9;
    top: 70%; 
    right:31%;
    width: 250px;
    height: 230px;
    border-radius: 4px;
    transition: transform .2s;

  }  
  .box3{
    position: absolute;
    background-color:#D9D9D9;
    top: 70%; left: 75%;
    width: 250px;
    height: 230px;
    border-radius: 4px;
    transition: transform .2s;

  }
  .box1:hover{
    transform: scale(1.05);
  }
  .box2:hover{
    transform: scale(1.05);

  }
  .box3:hover{
    transform: scale(1.05);
  }

  .home:hover{
    transform: scale(1.05);
  }


  body{
    background-color: #2D2D2F;
  }

</style>