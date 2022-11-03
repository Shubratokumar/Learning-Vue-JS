<template lang="">
    <div>
        <h3>This is Student Component.</h3>
        <h4>Student Name is : {{name}}</h4>
    </div>
</template>
<script>
export default {
    name: "Student",
    props:{
        name: String
    }
}
</script>
<style lang="">
    
</style>