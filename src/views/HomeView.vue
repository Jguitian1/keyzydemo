<template>
  <router-view/>
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
    <div class = "textContainer1">
      
      <span>Dishonred 2</span><br>
      <div class = "button1">
        <p> $39.99 </p>
      </div>
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
    <div class = "textContainer2">
      <span>CyberPunk 2077</span><br>

      <div class = "button1">
        
        <p> $59.99 </p>
      </div>
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
    <div class = "textContainer3">
      <span>Rust</span><br>

      <div class = "button1">
        <p> $39.99 </p>
      </div>
    </div>
  </div>


</template>

<style scoped>

div{
  animation: fadeIn .5s;

}
@keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}
.home{
  position: absolute;
  background-image: url( "../assets/castle.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  top: 5%; right: 4.2%;
  width: 900px;
  height: 500px;
  border-radius: 4px;
  transition: transform .2s;
  display: grid;
  grid-template-columns: repeat(8, 1fr);
  gap: 10px;
  grid-auto-rows: 117.5px;
  grid-template-areas:
    "a a a a b b b b"
    "a a a a b b b b"
    "c c c d d d d d"
    "c c c d d d d d";
  justify-content: center;
  align-content: center;
  
  }
  .textArea{
    grid-area: c;
    height: 500px;
    width: 600px;
    align-self: end;
    background: linear-gradient(to left, transparent 0%, black 130%);
    border-radius: 4px;

  }
  .home > .textArea > p{
    color: white;
    font-size: 25px;
    font-family: 'Rubik', sans-serif;
    position: absolute;
    top: 250px;
    left: 25px;

  }
  .home > .textArea > span{
    color: white;
    font-size: 11px;
    font-family: 'Inter', sans-serif;
    position: absolute;
    top: 300px;
    left: 25px;
    width: 300px;

  }
  .button{
    background-color: white;
    position: absolute;
    top: 400px;
    left: 25px;
    width: 100px;
    border-radius: 4px;
    height: 25px;

  }
  .textContainer1 > .button1{
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
  
  .textContainer2 > .button1{
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
  
  .textContainer3 > .button1{
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
  .button > p{
    font-family: 'Inter', sans-serif;
    display: grid;
    justify-content: center;
    align-content: center;
    color: black;
  }
  .box1{
    position: absolute;
    background-image: url( "../assets/dis.jpg");
    background-repeat: no-repeat;
    background-size: cover;    
    top: 80%; right: 58.4%;
    width: 250px;
    height: 230px;
    border-radius: 4px;
    transition: transform .2s;
  }
  .box2{
    position: absolute;
    background-image: url( "../assets/cyb.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    top: 80%; 
    right:31%;
    width: 250px;
    height: 230px;
    border-radius: 4px;
    transition: transform .2s;

  }  
  .box3{
    position: absolute;
    background-image: url( "../assets/rust.jpg");
    background-size: cover;
    background-repeat: no-repeat;    
    top: 80%; left: 75%;
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
    position: absolute;
    border-radius: 4px;
    opacity: 0;
    z-index: 2;
    transition: 0.3s ease-out;
    height: 100%;
    width: 100%;
    background: linear-gradient(to top, transparent 0%, black 130%);

  }
  .box2 .img-description{
    position: absolute;
    border-radius: 4px;
    opacity: 0;
    z-index: 2;
    transition: 0.3s ease-out;
    height: 100%;
    width: 100%;
    background: linear-gradient(to top, transparent 0%, black 130%);

  }
  .box3 .img-description{
    position: absolute;
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
    position: absolute;
    top: 110%; right: 58.4%;
    width: 250px;
    height: 125px;
    color: white;
    font-family: 'Rubik', sans-serif;
    font-size: 20px;
  }
  .textContainer2{
    position: absolute;
    top: 110%;
    right:31%;
    width: 250px;
    height: 125px;
    color: white;
    font-family: 'Rubik', sans-serif;
    font-size: 20px;
  }
  .textContainer3{
    position: absolute;
    top: 110%; left: 75%;
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