<template>
    <div class="drawer-toggle" role="button" @click="$emit('toggle')"> <img src="https://static.thenounproject.com/png/2292434-200.png" />
        <div class="bar"></div>
        <div class="bar"></div>
        <div class="bar"></div>
    </div>
</template>

<script>

export default {
    name:"TheSidebarToggle",
    props:{
        show:{
            type:Boolean,
            default:false
        }
    }
}
</script>


<style scoped>


.drawer-toggle{
    display: flex;
    flex-direction: columns;
    justify-content: space-around;
    height: 50%;
    width: 35px;
    cursor: pointer;
}
</style>