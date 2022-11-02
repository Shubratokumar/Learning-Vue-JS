<template>
<div>
    <h1>Home Component </h1>
    <h2>Name: {{getName("Shubrato Kumar")}}</h2>
    <h4>Email: {{ email }}</h4>
    <h4>Mobile: {{ mobile }}</h4>
    <!-- assign values -->
    <h4>Mobile1: {{ mobile= '+880180123456' }}</h4>
    <!-- comparision -->
    <h4>Mobile2: {{ mobile=='+880180123456' }}</h4>
    <h5>Sum : {{ 10 + 15  }}</h5>
    <h6>String Length : {{"Hello".length}}</h6>
</div>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            email: "shubrato@gmail.com",
            mobile: '+8801701234567',
            getName: function (name) {
                return name
            }
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
