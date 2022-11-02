<template>
<div>
    <h1>Pass data from parent to child component</h1>
    <Child name="Data passed from parent to child component" :user="user" :getData="getData"/>  
</div>
</template>

<script>
import Child from "./Child.vue"
export default {
    name: "Home",
    components: {
        Child
    },
    data() {
        return {            
            user: [
                {
                    name: "Shubrato",
                    email: "shubrato@gmail.com"
                },
                {
                    name: "Shuvo",
                    email: "shuvo@gmail.com"
                },
                {
                    name: "Shovan",
                    email: "shovan@gmail.com"
                },
            ]
        }
    },
    methods: {
        getData(){
            alert("Function called at child component which passed from parent component.")
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
