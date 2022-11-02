<template>
<div>
    <input type="text" v-model="data">
    <h4>Data: {{data}}</h4>

</div>
</template>

<script>
export default {
    name: "Home",
    data(){
        return{
            data: "No Data Here!"
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
