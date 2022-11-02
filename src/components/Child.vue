<template >
    <div>
        <h2>Hello from Child Component</h2>
        <h2>{{name}}</h2>
        <!-- User data -->
        <br>
        <h2>User Data</h2>
        <h3>{{user.name}}</h3>
        <h3>{{user.email}}</h3>
        
    </div>
</template>
<script>
export default {
    name: "Child",
    props: {
        name: String,
        user: Object
    }    
}
</script>
<style lang="">
    
</style>