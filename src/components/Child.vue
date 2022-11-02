<template>
<div>
    <h2>Hello from Child Component</h2>
    <h2>{{name}}</h2>
    <!-- User data -->
    <br>
    <h2>User Data</h2>
    <ul>
        <li v-for="item in user" key="item.email">
            Name : {{item.name}} and Email : {{item.email}}
        </li>
    </ul>
    <br>
    <!-- function call -->
    <button v-on:click="getData()">Call Function</button>
</div>
</template>

<script>
export default {
    name: "Child",
    props: {
        name: String,
        user: Array,
        getData: Function
    }
}
</script>

<style lang="">

</style>
