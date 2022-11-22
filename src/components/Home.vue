<template>
    <div>
        <h1>Dynamic Components in Vue js 3</h1>
        <button @click="tab='Php'">Load Php</button>
        <button @click="tab='JavaScript'">Load JavaScript</button>
        <button @click="tab='Java'">Load Java</button>
        <button @click="tab='Node'">Load Node</button>
        <component :is="tab" />
    </div>
</template>

<script>
import Php from "./Php.vue";
import JavaScript from "./JavaScript.vue";
import Node from "./Node.vue";
import Java from "./Java.vue";
export default {
    name: "Home",
    components:{
        Php, JavaScript, Node, Java
    },
    data() {
        return {
            tab: "JavaScript"
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
