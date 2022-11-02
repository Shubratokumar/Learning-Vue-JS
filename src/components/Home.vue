<template>
<div>
    <h1>For Loop in Vue JS</h1>
    <!-- simple array for loop -->
    <h3>Technology List : </h3>
    <ul>
        <li v-for="item in technology" :key="item">
            {{item}}
        </li>
    </ul>
    <br>
    <br>
    <h3>User Information List : </h3>
    <ul>
        <li v-for="item in user" :key="item.email">
            Name : {{item.name}} and Email : {{item.email}}
        </li>
    </ul>

</div>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            technology: [ "JS","React","Vue","Angular"," Node", " PHP"],
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
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
