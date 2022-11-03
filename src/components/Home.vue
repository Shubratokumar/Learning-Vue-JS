<template>
<div>
    <h1>Simple Form</h1>
    <p>{{form}}</p>
    <form action="">
        <label for="">Email :</label>
        <input type="text" placeholder="Enter Email" v-model="form.email">
        <br>
        <label for="">Password :</label>
        <input type="password" placeholder="Enter Password" v-model="form.password">
        <br>
        <label for="">Country :</label>
        <select  v-model="form.country">
            <option >India</option>
            <option >Bangladesh</option>
            <option >USA</option>
        </select>
        <br>
        <h4>Technology: </h4>
        <label for="">Java :</label>
        <input type="checkbox" value="Java" v-model="form.technology">
        <br>
        <label for="">JavaScript :</label>
        <input type="checkbox" value="JavaScript" v-model="form.technology">
        <br>
        <h4>Gender: </h4>
        <label for="">Male :</label>
        <input type="radio" value="Male" name="gender" v-model="form.gender">
        <br>
        <label for="">Female :</label>
        <input type="radio" value="Female" name="gender" v-model="form.gender">
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
                password: "",
                country: "",
                technology: [],
                gender: ""
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
