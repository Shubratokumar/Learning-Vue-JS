<template>
<div>
    <h1>Reuse Componet</h1>
    <ul>
        <li v-for="item in users" :key="item.name">
            <User :data="item" :getData="getData"/>
        </li>
    </ul>
</div>
</template>

<script>
import User from "./User.vue"
export default {
    name: "Home",
    components: {
        User
    },
    data(){
        return{
            users:[
                { name: "Shubrato",email: "shubrato@gmail.com"},
                { name: "Shuvo",email: "shuvo@gmail.com"},
                { name: "Shovan",email: "shovan@gmail.com"},
                { name: "Tonmoy",email: "tonmoy@gmail.com"},
                { name: "JH",email: "jh@gmail.com"},
                { name: "SK",email: "sk@gmail.com"},
            ]
        }
    },
    methods:{
        getData(name){
            alert(`Function called by ${name}`)
        }
    }
    
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
