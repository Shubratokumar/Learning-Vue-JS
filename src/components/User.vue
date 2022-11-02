<template >
    <div class="user">
        <h2>Name: {{data.name}}</h2>
        <h3>Email: {{data.email}}</h3>
        <button v-on:click="getData(data.name)">Alert Message</button>
    </div>
</template>
<script>
export default {
    name: "User",
    props:{
        data: Object,
        getData: Function
    }
}
</script>
<style scoped>
    .user{
        background-color: skyblue;
        padding: 10px;
        border-bottom: 1px solid orangered;
        margin-bottom: 20px;
    }
</style>