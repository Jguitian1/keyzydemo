<template>
  <div class="home">
      <div class = "game2">
        <p style="font-size: 36px; font-weight: bold;font-family: 'Rubik', sans-serif; margin-left: 25px;margin-top: 20px;">
          Castle Crashers
        </p>
        <p style="font-size: 11px; margin-top: 10px;margin-left: 25px; width: 50%;"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac risus ac quam cursus egestas sed in orci. Duis tempor libero nulla.  Ut eu interdum felis. Fusce quis lobortis lorem, eget consequat ligula. Etiam at porta neque. Sed quis tincidunt justo. Fusce lorem nisi.
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac risus ac quam cursus egestas sed in orci. Duis tempor libero nulla.  Ut eu interdum felis. Fusce quis lobortis lorem, eget consequat ligula. Etiam at porta neque. Sed quis tincidunt justo. Fusce lorem nisi.
        </p>
        <div style="height: 10px;width: 10px; margin-left: 25px"/>
        <div class="launch">
          <img src = "./imgs/play.svg" style="margin-left: 3px;"/>
          <p style="margin-top: 5px; font-size: 14px; margin-left: 4px;"> LAUNCH </p>

        </div>
        <p style="font-size: 36px; font-weight: bold;font-family: 'Rubik', sans-serif; margin-top: 50px;margin-left: 25px;">
          Updates
        </p>
      </div>
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

.game2{
  display: flex;
  flex-direction: column;
  background-color: #D9D9D9;
  border-radius: 15px;
  height: 93vh;
  margin-top: 2vh;
  align-items: flex-start;
  align-content: center;
  transition: 0.3s;
  background-image: url("imgs/corn.jpg");
  background-position: center; /* Center the image */
  background-size:cover;
}

body{
  background-color: #2D2D2F;
  text-decoration: none;
}
.launch{
  width: 100px;
  display: flex;
  height: 35px;
  border-radius: 15px;
  background-color: #266DD3;
  transition: 0.3s;
  margin-left: 25px;


}

.launch:hover{
  transform: scale(1.2);
  cursor: pointer;

}


a {
  color: white;
  text-decoration: none;
}
</style>
