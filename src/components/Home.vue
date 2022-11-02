<template>
<div>
    <h1>HTML Binding</h1>
    <h3>Name: {{text}}</h3>
    <div v-html="tag"></div>
    <div v-html="email"></div>

</div>
</template>

<script>
export default {
    name: "Home",
    data(){
        return{
            text: "Anil Sidhu",
            tag: "Name: <h4> Shubrato </h4>",
            email: "Email: <h4> Shuvo@gmil.com </h4>",
        }
    },
    
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
