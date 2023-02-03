<template>
  <div class = cont>
    <div class="home">
    </div>
    <div class ="grid">
      <div class = "row">
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
      </div>
      <div class = "row">
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
      </div>
      <div class = "row">
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
      </div>
      <div class = "row">
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
        <div class = "box"></div>
      </div>
    </div>
  </div>
</template>
  
  <style scoped>
  .grid{
    display: flex;
    flex-direction: column;

  }
  .box{
    background-color:#D9D9D9;
    border-radius: 15px;
    width: 150px;
    height: 135px;
    margin-top: 15px;
    margin-left: 10px;
    margin-right: 10px;
    transition: 0.3s ease-out;

  }
  .cont{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-left: 200px;
  }

  .home{
    background-color:#D9D9D9;
    border-radius: 15px;
    width: 830px;
    height: 100px;
    margin-top: 15px;

    }
    body{
      background-color: #2D2D2F;
    }

    .box:hover{
      transform: scale(1.05);
      cursor: pointer;
    }
  
  </style>