<template>
<div>
    <h1>If-else conditions in Vue JS</h1>
    <h2 v-if="show">If-else condition</h2>
    <!-- <h2 v-else>Else Condition</h2> -->
    <button v-on:click="show=!show">{{show ? "Hide" : "Show"}}</button>

</div>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            show: false,
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
