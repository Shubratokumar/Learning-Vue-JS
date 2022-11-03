<template>
<div>
    <h1>Non Props Data</h1>
    <User data="Some Data" id="user-cmp"/>    
</div>
</template>

<script>
import User from "./User.vue";
export default {
    name: "Home",
    components:{
        User
    },
    data() {
        return {
            data: ""
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}

.purple {
    background-color: rebeccapurple;
    color: chartreuse;
    width: 250px;
    padding: 10px;
}

.other {
    font-size: 34px;
}

.err {
    color: red
}
</style>
