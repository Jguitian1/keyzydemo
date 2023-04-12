<script>
import { defineComponent } from 'vue'
import { Carousel, Navigation, Slide } from 'vue3-carousel'

import '../../node_modules/vue3-carousel/dist/carousel.css'

export default defineComponent({
  name: 'BreakPoints',
  components: {
    Carousel,
    Slide,
    Navigation,
  },
  data: () => ({
    // carousel settings
    settings: {
      itemsToShow: 1,
      snapAlign: 'center',
    },
    // breakpoints are mobile first
    // any settings not specified will fallback to the carousel settings
    breakpoints: {
      // 700px and up
      700: {
        itemsToShow: 3.5,
        snapAlign: 'center',
      },
      // 1024 and up
      1024: {
        itemsToShow: 4,
        snapAlign: 'start',
      },
    },
    images: [
                    {
                        id: '1',
                        big: "https://cdn.cloudflare.steamstatic.com/steam/apps/204360/ss_57cdabd9ae140e33c5551ee0088d1e5db11b4622.1920x1080.jpg?t=1666985972",
                        thumb: "https://upload.wikimedia.org/wikipedia/en/9/9f/Cyberpunk_2077_box_art.jpg"
                    },
                    {
                        id: '2',
                        big: 'https://static.kinguin.net/cdn-cgi/image/w=1140,q=80,fit=scale-down,f=auto/media/category/2/-/2-1024_457.jpg',
                        thumb: 'https://static-cdn.jtvnw.net/ttv-boxart/263490_IGDB-272x380.jpg'
                    },
                    {
                        id: '3',
                        big: 'https://cdn.akamai.steamstatic.com/steam/apps/204360/ss_9cf7ff6ba267da33e140f66c29f50fd2ed391da2.1920x1080.jpg?t=1666985972',
                        thumb: 'https://image.api.playstation.com/vulcan/ap/rnd/202009/2918/1UfdyQmXpeSdoFE104sNkLd4.png'
                    },
                    {
                        id: '4',
                        big: 'https://cdn.akamai.steamstatic.com/steam/apps/204360/ss_a6a154f004bd7d0c3c7c1a0b378216ce0e8c8dd2.1920x1080.jpg?t=1666985972',
                        thumb: 'https://store-images.s-microsoft.com/image/apps.13950.70702278257994163.eb8febd9-1124-4e74-9587-d5082fbfffb5.5422b74c-3e78-408f-8df6-9a88c288b704'
                    },
                    {
                        id: '5',
                        big: 'https://cdn.akamai.steamstatic.com/steam/apps/204360/ss_2f53c16cb83d492cae0421ca090d2591f863e448.1920x1080.jpg?t=1666985972',
                        thumb: 'https://image.api.playstation.com/vulcan/ap/rnd/202206/0300/E2vZwVaDJbhLZpJo7Q10IyYo.png'
                    },

                ]
    
  }),
})
</script>

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

  <div class="pillArea">
    <div class = "pill1">
      FREE TO PLAY
    </div>
    <div class = "pill">
      RPG
    </div>
    <div class = "pill">
      ROLE PLAYING
    </div>
    <div class = "pill">
      JRPG
    </div>
    <div class = "pill">
      RACING
    </div>
    <div class = "pill">
      STORY
    </div>
    <div class = "pill">
      MMO
    </div>
    <div class = "pill">
      SANDBOX
    </div>
    <div class = "pill">
      LAN
    </div>

  </div>

  <div class = "heading">
    FREE TO PLAY
  </div>

  <div class="boxcont">
    <Carousel v-bind="settings" :breakpoints="breakpoints" :wrap-around="true">
      <Slide v-for="(image) in  images" :key="image.id">
        <div class="carousel__item"> 
          <img class="carousel__item" :src="image.thumb"> 
        </div>
      </Slide>
  
      <template #addons>
        <Navigation />
      </template>
    </Carousel>
  </div>

  <div class = "heading">
    RECOMENDED
  </div>
  <div class ="saleCont">
    <div class = "sale">
    </div>
    <div class = "stackedSale">
        <div class = "stacked"></div>
        <div class = "stacked1"></div>
        <div class = "stacked2"></div>
        <div class = "stacked3"></div>

    </div>
  </div>
  <div class = "heading">
    RPG
  </div>

  <div class="boxcont">
    <Carousel v-bind="settings" :breakpoints="breakpoints" :wrap-around="true">
      <Slide v-for="(image) in  images" :key="image.id">
        <div class="carousel__item"> 
          <img class="carousel__item" :src="image.thumb"> 
        </div>
      </Slide>
  
      <template #addons>
        <Navigation />
      </template>
    </Carousel>
  </div>
  </div>
</template>
<style>
.carousel__item {
  width: 200px;
  height: 250px;
  background-color: red;
  padding: 0px;
  margin: 0px;
  border-radius: 10px;
}
.carousel__slide{
  width: 100px;

}
.carousel__viewport {
  overflow: hidden;
  width: 900px;
}

.carousel__prev, .carousel__next {
  margin: 0 -40px;
  color: #D9D9D9;

}
</style>>


<style scoped>
.heading{
  color:white;
  font-family: 'Rubik', sans-serif;
  font-size: 24px;
  font-weight: 100;
  display: flex;
  width:1000px;
  margin-left: 300px;
  margin-top: 15px;
}
.pillArea{
  width: 900px;
  margin-top: 35px;
  display: flex;
  margin-left: 200px;
  gap:20px;
}
.pill1{
  color:rgb(255, 255, 255);
  font-size: 11px;
  font-family: 'Inter', sans-serif;
  height: 25px;
  text-decoration: underline;
  cursor: default;
  
}
.pill{
  color:rgb(168, 168, 168);
  font-size: 11px;
  font-family: 'Inter', sans-serif;
  height: 25px;
  cursor: pointer;

}
.saleCont{
  width: 900px;
  display: flex;
  height: 300px;

  margin-left: 200px;
  margin-bottom: 15px;

}
.sale{
  background-color: #D9D9D9;
  background-image: url("../assets/cyberpunk.jpg");
  width: 695px;
  margin-right: 5px;
  height: inherit;
  border-radius: 15px;
  transition: .1s ease-in;
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
.stackedSale{
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.stacked{
  width: 200px;
  height: 70px;
  background-color: #D9D9D9;
  border-radius: 15px;
  background-image: url("./imgs/cyberpunk.jpg");
  background-size: cover;
}
.stacked1{
  width: 200px;
  height: 70px;
  background-color: #D9D9D9;
  border-radius: 15px;
  background-image: url("./imgs/dis.jpg");
  background-size: cover;
}
.stacked2{
  width: 200px;
  height: 70px;
  background-color: #D9D9D9;
  border-radius: 15px;
  background-image: url("./imgs/rust.jpg");
  background-size: cover;
}
.stacked3{
  width: 200px;
  height: 70px;
  background-color: #D9D9D9;
  border-radius: 15px;
  background-image: url("./imgs/castle.jpg");
  background-size: cover;
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
  background-position: 0px;
  display: flex;
  flex-direction: column;
  background-size: cover;
  width: 900px;
  height: 300px;
  border-radius: 4px;
  transition: transform .2s;
  margin-left: 200px;

  }

  .boxcont{
    margin-top: 25px;
    display: flex;
    margin-left: 200px;
    margin-bottom: 25px;
  }
  .textArea{
    display: flex;
    flex-direction: column;
    height: inherit;
    width: inherit;
    align-self: end;
    background: linear-gradient(to left, transparent 0%, black 130%);
    border-radius: 4px;

  }
  .home > .textArea > p{
    color: white;
    margin-left: 25px;
    font-size: 25px;
    font-family: 'Rubik', sans-serif;
    margin-top: 100px;

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

