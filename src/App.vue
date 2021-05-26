<template>
  <div id="app">
    <div id="nav">
      <Navbar/>
    </div>
   
      <div id="login" >
        
          <transition
              name="fade"
              mode="out-in"
          >
            <router-view/>
          </transition>
      

      </div>

   

  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'


export default{
  components: { Navbar },

}

</script>


<style>

#login{
  align-items: center;
  display:flex;
  justify-content: center;
  align-items: center;
}

#app {
  font-family: "Poppins",Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width:100%;
}

#nav{
  width: 100% !important;
}


#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}


* {
  box-sizing: border-box;
}

.container{
  display:flex;
  justify-content:center;
}

body {
  
  min-height: 100vh;
  display: flex;
  font-weight: 400;
}

body,
html,
.App,
.vue-template,
.vertical-center {
  width: 100%;
  height: 100%;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}

.navbar-light {
  background-color: #ffffff;
  box-shadow: 0px 14px 80px rgba(34, 35, 58, 0.2);
}

.vertical-center {
  display: flex;
  text-align: center;
  justify-content: center;
  flex-direction: column;
}

.vertical-center .form-control:focus {
  border-color: #2554FF;
  box-shadow: none;
}

.vertical-center h3 {
  text-align: center;
  margin: 0;
  line-height: 1;
  padding-bottom: 20px;
}

label {
  font-weight: 500;
}

.forgot-password,
.forgot-password a {
  text-align: right;
  font-size: 13px;
  padding-top: 10px;
  color: #7a7a7a;
  margin: 0;
}

.forgot-password a {
  color: #2554FF;
}

.fade-enter-active,
.fade-leave-active {
  transition-duration: 0.3s;
  transition-property: opacity;
  transition-timing-function: ease;
}

.fade-enter,
.fade-leave-active {
  opacity: 0
}


</style>
