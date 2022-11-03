<template>
<div>
    <h1>Simple Form</h1>
    <form action="">
        <label for="">Email :</label>
        <input type="text" placeholder="Enter Email" v-model="form.email">
        <br>
        <label for="">Password :</label>
        <input type="password" placeholder="Enter Password" v-model="form.password">
        <br>
        <button v-on:click="login">Login</button>
    </form>

</div>
</template>

<script>
export default {
    name: "Home",
    data(){
        return{
            form: {
                email: "",
                password: ""
            }
        }
    },
    methods: {
        login() {
            console.log("Login Data", this.form)
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
