<template>
  <div class="home">
    <div class = "textArea">
      <p> Castle Crashers </p>
      <span> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Labore amet praesentium, veniam accusamus veritatis cum autem quibusdam laboriosam ex. Saepe dolor iste veniam voluptates quia deserunt sint quos repellat cupiditate. </span>
      <div class = "button">
        <p> Buy </p>
      </div>
    </div>
    
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
    top: 70%; right: 58.4%;
    width: 250px;
    height: 230px;
    border-radius: 4px;
    transition: transform .2s;
  }
  .box2{
    position: absolute;
    background-image: url( "../assets/cyberpunk.jpg");
    background-repeat: no-repeat;
    background-size: cover;    
    top: 70%; 
    right:31%;
    width: 250px;
    height: 500px;
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
    cursor: pointer;
  }



  body{
    background-color: #2D2D2F;
  }

</style>