<template lang="">
        <h4 v-bind="$attrs">Peter</h4>
        <h4>Bruch</h4>
        <h4>Anil</h4>
        <h4>Shidhu</h4>
        <h4>{{data}}</h4>
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
        data: String
    }
    
}
</script>
<style lang="">
    
</style>