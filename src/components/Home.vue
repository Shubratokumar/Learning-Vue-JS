<template>
<div>
    <h1>Watchers</h1>
    <h3>Counter : {{count}}</h3>
    <button v-on:click="count=count+1">+</button>

    <button v-on:click="count=count-1">-</button>

</div>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            count: 0
        }
    },
    watch: {
        count(val, prev) {
            // conditional watcher
            if (val > 5 && val > prev) {
                this.count = 0
            }
            // alert("Stop value changing")
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
