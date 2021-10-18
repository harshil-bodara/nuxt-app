<template>
    <header class="header">
            <TheSidebarToggle @toggle="$emit('sidenavToggle')"/>
            <ul class="nav-items">
                <li class="nav-item"><nuxt-link to="/">Home</nuxt-link></li>
                <li class="nav-item"><nuxt-link to="/posts">posts</nuxt-link></li>
                <li class="nav-item"><nuxt-link to="/about">About</nuxt-link></li>
                <li class="nav-item"><nuxt-link to="/admin">Admin</nuxt-link></li>
            </ul>
    </header>
</template>

<script>
import TheSidebarToggle from '~/components/navigation/TheSidebarToggle.vue'

export default {
    components:{
        TheSidebarToggle
    }
}
</script>


<style scoped>
.header{
    width: 100%;
    height: 60px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: rgb(173, 169, 167);
}
.nav-items{
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 80%;
}
.nav-items a{
    text-decoration: none;
    color: #000;
}
.nav-items a:hover,
.nav-items a:active,
.nav-item a.nuxt-link-active{
    color: red;
}

</style>