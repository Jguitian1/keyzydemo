<template>
<div class = "cont">
  <router-link to="/buy">
  <div class="home">
    <div class = "textArea">
      <p> Castle Crashers </p>
      <span> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Labore amet praesentium, veniam accusamus veritatis cum autem quibusdam laboriosam ex. Saepe dolor iste veniam voluptates quia deserunt sint quos repellat cupiditate. </span>
      <div class = "button">
        <p> Buy </p>
      </div>
    </div>
  </div>
  </router-link>

  <div class="boxcont">
  <div class = "threeBox">
    <div class = "box1">
      <span class="img-description">
        <h2 style="color: white; display:grid; justify-content: center; ">
          Dishonred 2
        </h2>
        <p style="padding: 5px; color: white; text-align:center; font-family: 'Inter', sans-serif;">
Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam voluptatum nesciunt atque. Facere magnam sed laboriosam voluptatum, expedita nemo fugit ipsa ullam tempore autem
        </p>
      </span>
    </div>


    <div class = "box2">
      <span class="img-description">
        <h2 style="color: white; display:grid; justify-content: center; ">
          CyberPunk 2077
        </h2>
        <p style="padding: 5px; color: white; text-align:center; font-family: 'Inter', sans-serif;">
Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam voluptatum nesciunt atque. Facere magnam sed laboriosam voluptatum, expedita nemo fugit ipsa ullam tempore autem
        </p>
      </span>
    </div>


    <div class = "box3">
      <span class="img-description">
        <h2 style="color: white; display:grid; justify-content: center; ">
          Rust
        </h2>
        <p style="padding: 5px; color: white; text-align:center; font-family: 'Inter', sans-serif;">
Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam voluptatum nesciunt atque. Facere magnam sed laboriosam voluptatum, expedita nemo fugit ipsa ullam tempore autem
        </p>
      </span>
    </div>

  </div>


  </div>

  <div class = "textcont">
    <div class = "textContainer1">

      <span>Dishonred 2</span><br>
      <div class = "button1">
        <p> $39.99 </p>
      </div>
    </div>
    <div class = "textContainer2">
      <span>CyberPunk 2077</span><br>

      <div class = "button1">

        <p> $59.99 </p>
      </div>
    </div>
    <div class = "textContainer3">
      <span>Rust</span><br>

      <div class = "button1">
        <p> $39.99 </p>
      </div>
    </div>
  </div>
  <div class = "sale">

  </div>
  <div class="boxcont">
    <div class = "threeBox">
      <div class = "box1">
      <span class="img-description">
        <h2 style="color: white; display:grid; justify-content: center; ">
          Dishonred 2
        </h2>
        <p style="padding: 5px; color: white; text-align:center; font-family: 'Inter', sans-serif;">
Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam voluptatum nesciunt atque. Facere magnam sed laboriosam voluptatum, expedita nemo fugit ipsa ullam tempore autem
        </p>
      </span>
      </div>


      <div class = "box2">
      <span class="img-description">
        <h2 style="color: white; display:grid; justify-content: center; ">
          CyberPunk 2077
        </h2>
        <p style="padding: 5px; color: white; text-align:center; font-family: 'Inter', sans-serif;">
Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam voluptatum nesciunt atque. Facere magnam sed laboriosam voluptatum, expedita nemo fugit ipsa ullam tempore autem
        </p>
      </span>
      </div>


      <div class = "box3">
      <span class="img-description">
        <h2 style="color: white; display:grid; justify-content: center; ">
          Rust
        </h2>
        <p style="padding: 5px; color: white; text-align:center; font-family: 'Inter', sans-serif;">
Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam voluptatum nesciunt atque. Facere magnam sed laboriosam voluptatum, expedita nemo fugit ipsa ullam tempore autem
        </p>
      </span>
      </div>

    </div>


  </div>

  <div class = "textcont">
    <div class = "textContainer1">

      <span>Dishonred 2</span><br>
      <div class = "button1">
        <p> $39.99 </p>
      </div>
    </div>
    <div class = "textContainer2">
      <span>CyberPunk 2077</span><br>

      <div class = "button1">

        <p> $59.99 </p>
      </div>
    </div>
    <div class = "textContainer3">
      <span>Rust</span><br>

      <div class = "button1">
        <p> $39.99 </p>
      </div>
    </div>
  </div>

  </div>
</template>



<style scoped>

.sale{
  background-color: #D9D9D9;
  width: 900px;
  height: 150px;
  border-radius: 15px;
  margin-left: 200px;
  margin-bottom: 15px;
  transition: .3s ease-in;
}

.sale:hover{
  transform: scale(1.05);
  cursor: pointer;
}

.cont{
  display: flex;
  flex-direction: column;
  align-items: center;

}

.textcont{
  margin-left: 200px;



}
div{
  animation: fadeIn .5s;
  display: flex;

}
@keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}
.home{
  margin-top: 25px;
  background-image: url("imgs/castle.jpg");
  display: flex;
  flex-direction: column;
  background-size: cover;
  width: 900px;
  height: 500px;
  border-radius: 4px;
  transition: transform .2s;
  margin-left: 200px;

  }

  .boxcont{
    margin-top: 25px;
    display: flex;
    margin-left: 200px;
  }
  .textArea{
    display: flex;
    flex-direction: column;
    height: 500px;
    width: 600px;
    align-self: end;
    background: linear-gradient(to left, transparent 0%, black 130%);
    border-radius: 4px;

  }
  .home > .textArea > p{
    color: white;
    margin-left: 25px;
    font-size: 25px;
    font-family: 'Rubik', sans-serif;
    margin-top: 200px;

  }
  a{

    text-decoration: none;
  }
  .home > .textArea > span{
    margin-left: 25px;
    color: white;
    font-size: 11px;
    font-family: 'Inter', sans-serif;
    width: 300px;

  }
  .button{
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 15px;
    background-color: white;
    width: 100px;
    border-radius: 4px;
    height: 25px;
    margin-left: 25px;


  }

  .button > p{
    margin-top: 10px;
  }
  .textContainer1 > .button1{
    background-color: white;
    margin-top: 25px;
    margin-left:-75px;
    color: black;
    font-family: 'Inter', sans-serif;
    position: absolute;
    width: 100px;
    border-radius: 4px;
    height: 25px;
    display: grid;
    justify-content: center;
    align-items: center;
    font-size: 16px;

  }

  .textContainer2 > .button1{
    background-color: white;
    margin-top: 25px;

    color: black;
    font-family: 'Inter', sans-serif;
    position: absolute;
    width: 100px;
    border-radius: 4px;
    height: 25px;
    display: grid;
    justify-content: center;
    align-items: center;
    font-size: 16px;


  }

  .textContainer3 > .button1{
    margin-left:75px;
    margin-top: 25px;
    background-color: white;
    color: black;
    font-family: 'Inter', sans-serif;
    position: absolute;
    width: 100px;
    border-radius: 4px;
    height: 25px;
    display: grid;
    justify-content: center;
    align-items: center;
    font-size: 16px;

  }

  .textContainer1 > span{
    margin-left:-75px;
  }
  .textContainer3 > span{
    margin-left:75px;
  }
  .button > p{
    font-family: 'Inter', sans-serif;
    display: grid;
    justify-content: center;
    align-content: center;
    color: black;
  }
  .box1{
    margin-right: 50px;
    background-image: url("imgs/dis.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    width: 250px;
    height: 230px;
    border-radius: 4px;
    transition: transform .2s;
  }
  .box2{
    margin-right: 25px;
    margin-left: 25px;

    background-image: url( "imgs/cyb.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    top: 75%;
    right:31%;
    width: 250px;
    height: 230px;
    border-radius: 4px;
    transition: transform .2s;

  }
  .box3{
    margin-left: 50px;

    background-image: url( "imgs/rust.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    top: 75%; left: 75%;
    width: 250px;
    height: 230px;
    border-radius: 4px;
    transition: transform .2s;

  }
  .box1:hover{
    transform: scale(1.05);
    cursor: pointer;
  }
  .box1 .img-description{
    border-radius: 4px;
    opacity: 0;
    z-index: 2;
    transition: 0.3s ease-out;
    height: 100%;
    width: 100%;
    background: linear-gradient(to top, transparent 0%, black 130%);

  }
  .box2 .img-description{
    border-radius: 4px;
    opacity: 0;
    z-index: 2;
    transition: 0.3s ease-out;
    height: 100%;
    width: 100%;
    background: linear-gradient(to top, transparent 0%, black 130%);

  }
  .box3 .img-description{
    border-radius: 4px;
    opacity: 0;
    z-index: 2;
    transition: 0.3s ease-out;
    height: 100%;
    width: 100%;
    background: linear-gradient(to top, transparent 0%, black 130%);

  }
  .box2:hover{
    transform: scale(1.05);
    cursor: pointer;

  }
  .box1:hover .img-description {
    opacity: 1;
  }
  .box2:hover .img-description {
    opacity: 1;
  }
  .box3:hover .img-description {
    opacity: 1;
  }
  .box3:hover{
    transform: scale(1.05);
    cursor: pointer;
  }

  .home:hover{
    transform: scale(1.05);
    cursor: pointer;
  }
  .textContainer1{

    width: 250px;
    height: 125px;
    color: white;
    font-family: 'Rubik', sans-serif;
    font-size: 20px;
  }
  .textContainer2{
    top: 105%;
    right:31%;
    width: 250px;
    height: 125px;
    color: white;
    font-family: 'Rubik', sans-serif;
    font-size: 20px;
  }
  .textContainer3{
    top: 105%; left: 75%;
    width: 250px;
    height: 125px;
    color: white;
    font-family: 'Rubik', sans-serif;
    font-size: 20px;

  }


  body{
    background-color: #2D2D2F;
  }

</style>

