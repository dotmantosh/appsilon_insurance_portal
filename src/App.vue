<template>
  <v-app>
    <v-main>
      
        <div class="dashbord__container">
          <Sidebar/>
          <MainContent/>
        </div>

     
    </v-main>
  </v-app>
</template>

<script>
import Sidebar from './components/Sidebar.vue'
import MainContent from './components/MainContent.vue'


export default {
  name: 'App',
  components: {
    Sidebar,
    MainContent
  }
}
</script>

<style lang="scss">
:root{
--app-purple-1: #713BDB;
--app-purple-2: #A2A4B9;

--app-grey-1: #42474A;
}




@font-face {
  font-family: "Segoe UI";
  src: url("./assets/fonts/SEGOEUI.TTF");
}
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  font-size: 62.5% !important;
  box-sizing: border-box !important;
  overflow-y: auto !important;
}
body{
  
  width: 100%;
  height: 100vh;

  position: relative;
  height: inherit;
}
#app {
  font-family: "Segoe UI" !important;
  position: relative;
  height: inherit;
}
.v-main{
  background: #e5e5e5 !important;
}

.dashbord__container{
  width: 90vw;
  min-height: 95vh;
  position: absolute;
  top: 50%;
  left: 50%;
  background: #F4F5F9;
  transform: translate(-50%, -50%);
  border-radius: 20px;
  display: flex;
} 

</style>

