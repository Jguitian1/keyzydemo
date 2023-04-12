<template>
  <div class="home">
      <div class = "game2">
        <p style = "text-align: center; padding-left: 25px;padding-top: 10px; font-size: 14.5px;">
          CASTLE <br> CRASHERS
        </p>
        <div style="border-left: 1px solid #9b9b9b; height: 70px; margin-left: 25px; margin-right:25px;" />
        <p style="font-size: 11px; margin-top: 10px"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac risus ac quam cursus egestas sed in orci. Duis tempor libero nulla.  Ut eu interdum felis. Fusce quis lobortis lorem, eget consequat ligula. Etiam at porta neque. Sed quis tincidunt justo. Fusce lorem nisi.</p>
        <div style="height: 10px;width: 10px; margin-left: 25px"/>
        <div class="launch">
          <img src = "./imgs/play.svg" style="margin-left: 5px; height:22px;"/>
          <p style="margin-top: 15px; font-size: 14px; margin-left: 7px;"> LAUNCH </p>
        </div>
      </div>    
      


    <div class = "game3">
      <p style = "text-align: center; padding-left: 25px;padding-top: 10px;font-size: 12.5px;; ">
        CYBERPUNK <br> 2077
      </p>
      <div style="border-left: 1px solid #9b9b9b; height: 70px; margin-left: 25px; margin-right:25px;" />
      <p style="font-size: 11px; margin-top: 10px"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac risus ac quam cursus egestas sed in orci. Duis tempor libero nulla.  Ut eu interdum felis. Fusce quis lobortis lorem, eget consequat ligula. Etiam at porta neque. Sed quis tincidunt justo. Fusce lorem nisi.</p>
      <div style="height: 10px;width: 10px; margin-left: 25px"/>
      <div class="launch">
        <img src = "./imgs/play.svg" style="margin-left: 5px; height:22px;"/>
        <p style="margin-top: 15px; font-size: 14px; margin-left: 7px;"> LAUNCH </p>
      </div>
    </div>    
    
    <div class = "game4">
      <p style = "text-align: center; padding-left: 25px;padding-top: 10px; font-size: 13px; ">
        DISHONRED <br> 2
      </p>
      <div style="border-left: 1px solid #9b9b9b; height: 70px; margin-left: 25px; margin-right:25px;" />
      <p style="font-size: 11px; margin-top: 10px"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac risus ac quam cursus egestas sed in orci. Duis tempor libero nulla.  Ut eu interdum felis. Fusce quis lobortis lorem, eget consequat ligula. Etiam at porta neque. Sed quis tincidunt justo. Fusce lorem nisi.</p>
      <div style="height: 10px;width: 10px; margin-left: 25px"/>
      <div class="launch">
        <img src = "./imgs/play.svg" style="margin-left: 5px; height:22px;"/>
        <p style="margin-top: 15px; font-size: 14px; margin-left: 7px;"> LAUNCH </p>
      </div>
    </div>    
    <router-link to="/lib">

    <div class = "game5">
      <p style = "text-align: center; padding-left: 25px;padding-top: 10px; font-size: 28px;">
        RUST
      </p>
      <div style="border-left: 1px solid #9b9b9b; height: 70px; margin-left: 25px; margin-right:25px;" />
      <p style="font-size: 11px; margin-top: 10px"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac risus ac quam cursus egestas sed in orci. Duis tempor libero nulla.  Ut eu interdum felis. Fusce quis lobortis lorem, eget consequat ligula. Etiam at porta neque. Sed quis tincidunt justo. Fusce lorem nisi.</p>
      <div style="height: 10px;width: 10px; margin-left: 25px"/>
      <div class="launch">
        <img src = "./imgs/play.svg" style="margin-left: 5px; height:22px;"/>
        <p style="margin-top: 15px; font-size: 14px; margin-left: 7px;"> LAUNCH </p>
      </div>
    </div>    
  </router-link>

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
      height: 110px;
      margin-top: 13px;
      align-items: center;
      align-content: center;
      transition: 0.3s;
      background-image: url("imgs/castless.jpg");
      background-position: 0px; /* Center the image */
      background-size:cover;

    }
    .game3{
      display: flex;
      background-color: #D9D9D9;
      border-radius: 15px;
      height: 110px;
      margin-top: 13px;
      align-items: center;
      align-content: center;
      transition: 0.3s;
      background-image: url("imgs/cybss.jpg");
      background-position: 0px; /* Center the image */
      background-size:cover;

    }
    .game4{
      display: flex;
      background-color: #D9D9D9;
      border-radius: 15px;
      height: 110px;
      margin-top: 13px;
      align-items: center;
      align-content: center;
      transition: 0.3s;
      background-image: url("imgs/dishss.jpg");
      background-position: 0px; /* Center the image */
      background-size:cover;

    }
    .game5{
      display: flex;
      background-color: #D9D9D9;
      border-radius: 15px;
      height: 110px;
      margin-top: 13px;
      align-items: center;
      align-content: center;
      transition: 0.3s;
      background-image: url("imgs/rustss.jpg");
      background-position: 0px; /* Center the image */
      background-size:cover;

    }
    body{
      background-color: #2D2D2F;
      text-decoration: none;
    }
    .launch{
      width: 110px;
      display: flex;
      align-items: center;
      height: 35px;
      border-radius: 15px;
      background-color: #266DD3;
      margin-left: auto + 10px;
      padding-right: 100px;


    }

    .game:hover{
      transform: scale(1.01);
      cursor: pointer;

    }
    .game2:hover{
    transform: scale(1.005);
    cursor: pointer;

  }
  .game3:hover{
    transform: scale(1.005);
    cursor: pointer;

  }
  .game4:hover{
    transform: scale(1.005);
    cursor: pointer;

  }
  .game5:hover{
    transform: scale(1.005);
    cursor: pointer;

  }



a {
  color: white;
  text-decoration: none;
}

</style>
