<template>
  <div class="main-content">
    <Header/>
    <Reports/>
  </div>
</template>

<script>
import Header from './Header.vue'
import Reports from './Reports.vue'
export default {
  components:{
    Header,
    Reports
  }
}
</script>

<style>
.main-content{
  flex: 1;
}


</style>