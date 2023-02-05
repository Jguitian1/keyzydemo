<template>
  <div class="home">
    <router-link to="/lib">
      <div class = "game2">
        <p style = "text-align: center; padding-left: 25px;padding-top: 10px; ">
          Castle <br> Crashers
        </p>
        <div style="border-left: 1px solid #9b9b9b; height: 70px; margin-left: 25px; margin-right:25px;" />
        <p style="font-size: 11px; margin-top: 10px"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac risus ac quam cursus egestas sed in orci. Duis tempor libero nulla.  Ut eu interdum felis. Fusce quis lobortis lorem, eget consequat ligula. Etiam at porta neque. Sed quis tincidunt justo. Fusce lorem nisi.</p>
        <div style="height: 10px;width: 10px; margin-left: 25px"/>
        <div class="launch">
          <img src = "./imgs/play.svg" style="margin-left: 3px; height:25px;"/>
          <p style="margin-top: 5px; font-size: 14px; margin-left: 4px;"> LAUNCH </p>
        </div>
      </div>
    </router-link>
    <div class = "game"> </div>
    <div class = "game"> </div>
    <div class = "game"> </div>
    <div class = "game"> </div>
    <div class = "game"> </div>
    <div class = "game"> </div>
    <div class = "game"> </div>
    <div class = "game"> </div>
    <div class = "game"> </div>
    <div class = "game"> </div>
  </div>
</template>

<style scoped>

  .home{
    display: flex;
    flex-direction: column;
    color: white;
    font-family: 'Inter', sans-serif;
    font-size: 18px;
    padding-left: 225px;
    padding-right: 25px;
    padding-top: 10px;
    overflow: auto;
  }


    .game{
      display: flex;
      background-color: #D9D9D9;
      border-radius: 15px;
      height: 90px;
      margin-top: 13px;
      align-items: center;
      align-content: center;
      transition: 0.3s;
    }
    .game2{
      display: flex;
      background-color: #D9D9D9;
      border-radius: 15px;
      height: 90px;
      margin-top: 13px;
      align-items: center;
      align-content: center;
      transition: 0.3s;
      background-image: url("imgs/corn.jpg");
      background-position: 0px; /* Center the image */
      background-size:cover;

    }
    body{
      background-color: #2D2D2F;
      text-decoration: none;
    }
    .launch{
      width: 100px;
      display: flex;
      align-items: center;
      height: 35px;
      border-radius: 15px;
      background-color: #266DD3;
      margin-left: auto;
      padding-right: 100px;

    }

    .game:hover{
      transform: scale(1.01);
      cursor: pointer;

    }
    .game2:hover{
    transform: scale(1.01);
    cursor: pointer;

  }

a {
  color: white;
  text-decoration: none;
}

</style>
