<template lang="">
    <div >
        <h4 >Peter</h4>
        <h4>Bruch</h4>
        <h4>Anil</h4>
        <h4>Shidhu</h4>
        <h4 v-bind="$attrs">{{data}}</h4>
    </div>
</template>
<script>
export default {
    name: "User",
    // inheritAttrs: false,
    data(){
        return{
            userName: "Shubrato"
        }
    },
    props: {
        data: String,
        id: String
    }
    
}
</script>
<style lang="">
    
</style>