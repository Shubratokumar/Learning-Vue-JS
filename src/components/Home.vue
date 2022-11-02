<template>
<div>
    <h1>Get input value</h1>
    <input type="text" placeholder="Enter your email here" v-model="email">
    <br/>
    <br/>
    <input type="password" placeholder="Enter your password here" v-model="password">
    <br/>
    <br/>
    <button v-on:click="getData()" type="button">Get Values</button>

</div>
</template>

<script>
export default {
    name: "Home",
    data(){
        return {
            email: null,
            password: null,
        }
    },
    methods: {
        getData(){
            console.log("Values:", this.email, this.password)
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
