<template>
<div>
    <h1>Teleport Components in Vue js 3</h1>
    <teleport to='#footer'>
        <Footer />
    </teleport>
</div>
</template>

<script>
import Footer from "./Footer.vue";
export default {
    name: "Home",
    components: {
        Footer
    },
    data() {
        return {

        }
    },
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
