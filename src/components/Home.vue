<template>
<div>
    <h1 v-on:mousemove="getConsole()">Home Component </h1>
    <!-- <button v-on:click="getData(`Button single clicked`)">Click Me</button>
    <br>
    <button v-on:dblclick="getData(`Button 2X clicked`)">Click Me</button> -->
    <button v-on:click="getData()">Click Me</button>
    <h3>Counter : {{ count }}</h3>

</div>
</template>

<script>
export default {
    name: "Home",
    data(){
        return {
            count:0
        }
    },
    methods: {
        getData() {
            this.count= this.count+1
        },
        getConsole() {
            console.warn("function Called !!!")
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
