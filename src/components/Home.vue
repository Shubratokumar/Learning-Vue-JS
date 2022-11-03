<template>
<div>
    <h1>Computed Property</h1>
    <!-- Normal useage -->
    <h3>{{(dollors * tkVal) - discount}}</h3>   
    <h3>{{(dollors * tkVal) - discount}}</h3>   
    <h3>{{(dollors * tkVal) - discount}}</h3>
    <!-- computed property -->
    <h3>{{getResult}}</h3>   
    <h3>{{getResult}}</h3> 
    <!-- using methods must call the function  -->
    <h3>{{getResultMethods()}}</h3>   
</div>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            dollors: 100,
            tkVal: 95,
            discount: 10
        }
    },
    methods: {
        getResultMethods(){
            return (this.dollors * this.tkVal) - this.discount
        }
    },
    computed: {
        getResult(){
             return (this.dollors * this.tkVal) - this.discount
        }
    }

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
