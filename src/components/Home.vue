<template>
<div>
    <h1>Props in Vue JS </h1>
    <Teacher :name="namet"/>
    <Student :name="names"/>

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
            namet: "Jhankar",
            names: "Shuvo"

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
