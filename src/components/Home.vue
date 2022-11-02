<template>
<div>
    <h1>Class Binding</h1>
    <h3 :class="applyStyle">This is Home</h3>
    <button v-on:click="colorfull=!colorfull">{{colorfull ? "Remove style" : "Apply style"}}</button>

</div>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            colorfull: false,
        }
    },
    computed: {
        applyStyle() {
            return {
                purple: this.colorfull,
                err: true,
                other: true
            }
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
