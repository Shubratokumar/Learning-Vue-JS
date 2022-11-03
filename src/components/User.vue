<template lang="">
    <div>
        <h2>User Component as Child</h2>
        <button v-on:click="getUser(userName)">Send User Name</button>
    </div>
</template>
<script>
export default {
    name: "User",
    data(){
        return{
            userName: "Shubrato"
        }
    },
    props: {
        getUser: Function
    }
    
}
</script>
<style lang="">
    
</style>