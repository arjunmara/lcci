<template>
  <div class="about">
    <my-navbar></my-navbar>
    <h1>This is an about page</h1>
    <my-footer></my-footer>
  </div>
</template>
<script>
import myNavbar from '../components/Navbar.vue'
import myFooter from '../components/Footer.vue'
export default {
  name:'home',
  data:function(){
    return{
      
    }
  },
  components:{
    myNavbar,
    myFooter
  }
}
</script>