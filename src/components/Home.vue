<template>
<div>
    <h1>Slots in Vue js 3</h1>
    <Child1><h2>Shubrato</h2></Child1>
    <Child1><a href="#">Shubrato with link</a></Child1>
    <Child1><img src="https://images.unsplash.com/photo-1526547541286-73a7aaa08f2a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxleHBsb3JlLWZlZWR8Mnx8fGVufDB8fHx8&w=500&q=80"/></Child1>

</div>
</template>

<script>
import Child1 from "./Child1.vue"
export default {
    name: "Home",
    components:{
        Child1
    },
    data() {
        return {

        }
    },    
}
</script>

<style scoped>
h1 {
    color: orange;
}

.purple {
    background-color: rebeccapurple;
    color: chartreuse;
    width: 250px;
    padding: 10px;
}

.other {
    font-size: 34px;
}

.err {
    color: red
}
</style>
