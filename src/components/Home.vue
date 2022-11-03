<template>
<div>
    <h1>Props in Vue JS </h1>
    <Teacher name="Jhanka"/>
    <Student name="Shubrato"/>

</div>
</template>

<script>
import Student from "./Student.vue";
import Teacher from "./Teacher.vue";
export default {
    name: "Home",
    components: {
        Student,
        Teacher
    },
    data() {
        return {

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
