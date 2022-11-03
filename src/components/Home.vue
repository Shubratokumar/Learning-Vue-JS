<template>
<div>
    <h1>Form Modifiers</h1>
    <input type="text" v-model.trim="data">
    <h3>Data is: {{data}}</h3>
</div>
</template>

<script>
export default {
    name: "Home",
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
