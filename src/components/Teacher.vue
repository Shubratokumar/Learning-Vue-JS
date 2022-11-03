<template lang="">
    <div>
        <h3>This is Teacher Component.</h3>
        <h4>Teacher Name is : {{name}}</h4>
    </div>
</template>
<script>
export default {
    name: "Teacher",
    props:{
        name: String
    }

}
</script>
<style lang="">
    
</style>