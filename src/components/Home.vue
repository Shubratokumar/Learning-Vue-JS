<template>
<div>
    <h1>Class Binding</h1>
    <h3 :class="{purple:colorfull}">This is Home</h3>
    <button v-on:click="colorfull=!colorfull">{{colorfull ? "Remove style" : "Apply style"}}</button>


</div>
</template>

<script>
export default {
    name: "Home",
    data(){
        return{
            colorfull: !true,
        }
    },
    
}
</script>

<style scoped>
h1 {
    color: orange;
}
.purple{
    background-color: rebeccapurple;
    color: chartreuse;
    width: 200px;
    padding: 10px;
}
</style>
