<template>
    <div class="myDashboard">
        <myDashNav></myDashNav>
        <dash-content></dash-content>
    </div>
</template>
<script>
import myDashNav from '../components/DashNav.vue'
import DashContent from '../components/DashContent.vue'
export default {
    name:'dashboard',
    components:{
        myDashNav,
        DashContent
    }
}
</script>
