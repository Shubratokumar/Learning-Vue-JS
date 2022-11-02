<template>
<div>
    <h1>Home Component </h1>
    <h3>Email: {{ email }}</h3>
    <h3>First Name: {{ getName("Shubrato") }}</h3>
    <h3>Last Name: {{ getName("Kumar") }}</h3>
    <h4>All data: {{ getData()}}</h4>
    <h4>Email2: {{getData().email}}</h4>
    <h4>Name2: {{getData().name}}</h4>

</div>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            email: "shubrato@gmail.com",
        }
    },
    methods: {
        getName(name){
            return name;
        },
        getData(){
            return{
                name: "Shuvo",
                email: "shuvo@gmail.com"
            }
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
