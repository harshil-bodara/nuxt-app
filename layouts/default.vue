<template>
    <div>
        <Header @sidenavToggle="displaySideNav = !displaySideNav"/>
        <Sidebar :show="displaySideNav" @close="displaySideNav = false"/>
        <nuxt/>
    </div>
</template>

<script>
import Header from '~/components/navigation/TheHeader.vue'
import Sidebar from '~/components/navigation/TheSidebar.vue'


export default {
    components:{
        Header,
        Sidebar       
    },
    data(){
        return{
            displaySideNav:false
        }
    }
}
</script>

<style>
html{
    font-family: 'sans-serif', 'Open Sans';
}
body{
    margin: 0;
}

</style>