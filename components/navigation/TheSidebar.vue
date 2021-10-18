<template>
    <div class="sidebar-container">
        <div v-if="show" class="sidenav-backdrop" @click="$emit('close')">
            <transition name="slide-side">
                <div v-if="show" class="sidenav">
                    <ul class="nav-list" @click="$emit('close')">
                        <li class="nav-item"><nuxt-link to="/">Home</nuxt-link></li>
                        <li class="nav-item"><nuxt-link to="/about">About</nuxt-link></li>
                        <li class="nav-item"><nuxt-link to="/admin">Admin</nuxt-link></li>
                    </ul>
                </div>
            </transition>
        </div>
    </div>
</template> 

<script>

export default {
    name:"TheSidebar",
    props:{
        show:{
            type:Boolean,
            default:false
        }
    }
}
</script>


<style scoped>


.sidebar-container{
    width: 100%;
    height: 100%;
}
.sidebar-backdrop{
    width: 100%;
    height: 100%;
    background: cornflowerblue;
    position: fixed;
    z-index: 1000;
    top:0;
    left: 0;
}
.sidenav{
    height: 100%;
    width: 300px;
    background: white;
    z-index: 1000;
    position: fixed;
    top:0;
    left:0;
    box-sizing: border-box;
    padding: 30px;
}
.slide-slide-enter-active .slide-slide-leave-active {
    transition: all .3s ease-out;
}
.slide-side-enter .slide-side-leave-to{
    transform: translateX(-100%);
}

.nav-list{
    list-style: none;
    padding: 0;
    margin: 0;
}
.nav-item{
    margin:20px 0px;
}
.nav-item a {
    text-decoration: none;
    color:#000;
}
.nav-item a:hover,
.nav-item a:active,
.nav-item a.nuxt-link-active{
    color: red;
}

</style>