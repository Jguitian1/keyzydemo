<script>
import CaroselThumb from '../components/CaroselThumb.vue'

export default {
  name: 'App',
  components: {
    CaroselThumb
  }
}
</script>

<template>

  <div class="cont">
    <span class = "title"> Castle Crashers</span>
    <CaroselThumb/>
    <div class = "textArea">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Incidunt eaque inventore explicabo nihil doloremque quisquam voluptate corporis vero ad nobis mollitia, dignissimos vitae neque et, quasi laudantium nesciunt harum iure?
        <br>
    </div>
    <div class="buttonSpace">
        <span>Buy Castle Crashers</span>
        <div class = "Purchased">
            <span>Owned</span>
        </div>

        
    </div>
  </div>

</template>

<style scoped>

.cont{
  margin-left: 225px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.title{
    margin-right: 530px;
    color: white;
    font-size: 35px;
    left: 300px;
    font-family: 'Rubik', sans-serif;
}

.textArea{ 
    left: 300px; top: 700px;
    transition-timing-function: ease-in;
    animation: fadeIn .5s;
    width: 800px;
    height: 200px;
    color: white;

}
.buttonSpace{
    background-color: #3D3D3F;
    width: 800px;
    transition-timing-function: ease-in;
    animation: fadeIn .5s;
    width: 800px;
    height: 50px;
    color: #eae6e5;
    border-radius: 4px;
    display: inline;
    margin-bottom: 25px;

}
.buttonSpace > span{
    font-size: 30px;
    font-family: 'Rubik', sans-serif; 
    padding-left: 10px;
    width: 10%;
    display: inline;
}
.Purchased{
    display: inline;
    text-align: center;
    background-color: #2D2D2F;
    border-style: solid;
    border-width: 3px;
    border-color: #eae6e5;
    font-size: 15px;
    font-family: 'Inter', sans-serif;
    margin-left: 400px;
    padding: 10px;
    justify-content: center;
    padding-top: 10px;
}
.Purchased > span{
    display: inline;
    
}
@keyframes fadeIn {
    0% { opacity: 0; }
    100% { opacity: 1; }
  }

</style>
