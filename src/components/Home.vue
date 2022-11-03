<template>
<div>
    <h1>Data transfer child to parent component</h1>
    <User :getUser="getUserName" />

</div>
</template>

<script>
import User from "./User.vue";
export default {
    name: "Home",
    components: {
        User,
    },
    methods: {
        getUserName(data) {
            alert(data)
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
