<template>
    <button 
        class="button"
        :class="btnstyle"
        v-bind="$attrs"
        v-on="$listners"
    ><slot/>
    </button>
</template>

<script>
export default {
    name:"AppButton",
    props:{
        btnstyle:{
            type:String,
            default:''
        }
    }
}
</script>

<style scoped>
.button{
    font: inherit;
    background: black;
    color: #fff;
    padding: 5px;
    cursor: pointer;
    border:1px solid black;
}
.button:hover,
.button:active{
    background: rgb(51,51,51);
    border:1px solid black;
}
.inverted{
    background-color:#fff;
    color:black;
    border:1px solid transparent;
}
.inverted:hover,
.inverted:active{
    color:#ccc;
    background-color: white;
    border:1px solid transparent;
}
.cancel{
    background-color: red;
    color:white;
    border: 1px solid transparent;
}
.cancel:hover,
.cancel:active{
    border-color: salmon;
    border:1px solid transparent;
    color:white;
}
</style>