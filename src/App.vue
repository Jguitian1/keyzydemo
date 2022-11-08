<script>
import { CDropdown } from '@coreui/vue';
import { CDropdownToggle } from '@coreui/vue';
import { CDropdownMenu } from '@coreui/vue';
import { CDropdownItem } from '@coreui/vue';
import '@coreui/coreui/dist/css/coreui.min.css'

export default {
  components: {
    CDropdown,
    CDropdownToggle,
    CDropdownMenu,
    CDropdownItem
  }
}
</script>

<template>
  <router-view/>

  <div class="container">
    
    <nav>
      <div class = "slector">
      <CDropdown>
      <CDropdownToggle color="dark" class="btn btn-primary rounded-0">Select Wallet</CDropdownToggle>
      <CDropdownMenu>
        <CDropdownItem href="#">My Wallet   </CDropdownItem>
        <CDropdownItem href="#">Meta Mask</CDropdownItem>
      </CDropdownMenu>
      </CDropdown>
      </div>
      <router-link to="/"><svg xmlns="http://www.w3.org/2000/svg" id="Isolation_Mode" data-name="Isolation Mode" viewBox="0 0 25 25" width="15" height="15" fill="#9b9b9b"><circle cx="7" cy="22" r="2"/><circle cx="17" cy="22" r="2"/><path d="M5.654,5,5.391,2.938A3.328,3.328,0,0,0,2.087,0H0V3H2.087a.331.331,0,0,1,.326.3l1.5,11.759A3.327,3.327,0,0,0,7.217,18H20.4L23.974,5ZM18.112,15H7.217a.329.329,0,0,1-.325-.3L6.037,8h14Z"/></svg>
Store</router-link>
      <router-link to="/about"><svg xmlns="http://www.w3.org/2000/svg" id="Layer_1" data-name="Layer 1" viewBox="0 0 25 25" width="15" height="15" fill="#9b9b9b"><path d="M23.98,21.566L16.756,1.967c-.276-.752-.828-1.352-1.556-1.688-.727-.338-1.542-.371-2.294-.094l-.939,.345c-.283,.104-.544,.246-.778,.423-.548-.585-1.326-.952-2.189-.952H3C1.346,0,0,1.346,0,3V24H12V9.305l5.408,14.672,6.572-2.41Zm-5.387-.154l-.965-2.619,2.816-1.033,.965,2.619-2.816,1.033Zm-1.657-4.495l-3.489-9.466,2.816-1.034,3.489,9.466-2.816,1.033ZM12.093,2.925c.112-.242,.312-.427,.563-.519l.939-.345c.112-.041,.229-.062,.345-.062,.143,0,.285,.031,.419,.093,.243,.112,.427,.312,.52,.564l.694,1.884-2.816,1.034-.695-1.885c-.092-.251-.081-.522,.031-.765Zm-2.093,.075v2h-3V2h2c.551,0,1,.448,1,1Zm-3,4h3v10h-3V7Zm-2,10H2V7h3v10ZM3,2h2v3H2V3c0-.552,.449-1,1-1Zm-1,17h3v3H2v-3Zm5,3v-3h3v3h-3Z"/></svg>
Libary</router-link>
      <router-link to="/inventory"><svg xmlns="http://www.w3.org/2000/svg" id="Layer_1" data-name="Layer 1" viewBox="0 0 25 25" width="15" height="15" fill="#9b9b9b"><path d="M9,11a1,1,0,0,1,1-1h4a1,1,0,0,1,0,2H10A1,1,0,0,1,9,11Zm15,7v1a5.006,5.006,0,0,1-5,5H5a5.006,5.006,0,0,1-5-5V18a5.009,5.009,0,0,1,4-4.9V12A8,8,0,0,1,8.015,5.073C8.013,5.048,8,5.026,8,5V4a4,4,0,0,1,8,0V5c0,.026-.013.048-.015.073A8,8,0,0,1,20,12v1.1A5.009,5.009,0,0,1,24,18ZM10,4.263a7.736,7.736,0,0,1,4,0V4a2,2,0,0,0-4,0ZM6,16.535a8.368,8.368,0,0,1,12,0V12A6,6,0,0,0,6,12ZM5,22h.026A4.948,4.948,0,0,1,4,19V15.184A3,3,0,0,0,2,18v1A3,3,0,0,0,5,22Zm10,0a3,3,0,0,0,2.874-2.188,6.432,6.432,0,0,0-11.748,0A3,3,0,0,0,9,22Zm7-4a3,3,0,0,0-2-2.816V19a4.948,4.948,0,0,1-1.026,3H19a3,3,0,0,0,3-3Z"/></svg>
Inventory</router-link>
      <router-link to="/market"><svg xmlns="http://www.w3.org/2000/svg" id="Bold" viewBox="0 0 25 25" width="15" height="15" fill="#9b9b9b"><path d="M24,10.091,22.751,4.307A5.466,5.466,0,0,0,17.382,0H6.618A5.466,5.466,0,0,0,1.249,4.307L.036,9.766,0,11.046a4.321,4.321,0,0,0,1,2.745V18.5A5.506,5.506,0,0,0,6.5,24h11A5.506,5.506,0,0,0,23,18.5V13.791a4.321,4.321,0,0,0,1-2.745ZM3,10.256l1.177-5.3A2.5,2.5,0,0,1,6.618,3H7V4.5A1.5,1.5,0,0,0,8.5,6h0A1.5,1.5,0,0,0,10,4.5V3h4V4.5A1.5,1.5,0,0,0,15.5,6h0A1.5,1.5,0,0,0,17,4.5V3h.382a2.5,2.5,0,0,1,2.441,1.958L21,10.256v.79a1.364,1.364,0,0,1-2.727,0,2.455,2.455,0,1,0-4.909,0,1.364,1.364,0,0,1-2.728,0,2.455,2.455,0,1,0-4.909,0,1.364,1.364,0,0,1-2.727,0ZM17.5,21H6.5A2.5,2.5,0,0,1,4,18.5V15.372c.122.011.239.037.364.037a4.367,4.367,0,0,0,3.818-2.253,4.362,4.362,0,0,0,7.636,0,4.367,4.367,0,0,0,3.818,2.253c.125,0,.242-.026.364-.037V18.5A2.5,2.5,0,0,1,17.5,21Z"/></svg>
Market</router-link>
    </nav>
  </div>
</template>

<style>
.slector{
  padding-top: 20px;
  padding-bottom: 10px;
}
#app{
  margin: 0px;

}
.container{
  background-color: #1D1D1F;
  margin: 0px;
  width: 200px;
  height: 100vh;
  position: fixed;

}
body{
  margin:0;
  background-color: #2D2D2F;
  

}


nav {
  background-color: #1D1D1F;
  display: grid;
  text-decoration: none;
  position: fixed;
  z-index: 10;
}

nav a {
  font-weight: bold;
  color: #9b9b9b;
  text-decoration: none;
  padding-bottom: 10px;
  padding-top: 10px;
  font-family: 'Inter', sans-serif;


}
nav a:hover {
  color: #eae6e5;
}
nav a.router-link-exact-active {
  color: #eae6e5;
}
nav a.router-link-exact-active svg{
  fill: #eae6e5;

}
.btn-dark{
  --cui-btn-color: rgba(255, 255, 255, 0.87);
  --cui-btn-bg: #4A4A4C;
  --cui-btn-border-color: #4A4A4C;
  --cui-btn-hover-color: #fff;
  --cui-btn-hover-bg: #5A5A5C;
  --cui-btn-hover-border-color: #5A5A5C;
  --cui-btn-focus-shadow-rgb: 100,112,132;
  --cui-btn-active-color: #fff;
  --cui-btn-active-bg: #5A5A5C;
  --cui-btn-active-border-color: #5A5A5C;
  --cui-btn-active-shadow: inset 0 3px 5pxrgba(0, 0, 21, 0.125);
  --cui-btn-disabled-color: rgba(255, 255, 255, 0.87);
  --cui-btn-disabled-bg: #4f5d73;
  --cui-btn-disabled-border-color: #4f5d73;
}
</style>
