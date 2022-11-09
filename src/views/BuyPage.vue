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
    <span class = "title"> Castle Crashers</span>
    <CaroselThumb/>
</template>

<style scoped>
.title{
    color: white;
    font-size: 35px;
    position: absolute;
    left: 300px;
    font-family: 'Rubik', sans-serif;

}
</style>
