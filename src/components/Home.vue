<template>
<div>
    <h1>Multiple Slots in Vue js 3</h1>
    <Child1>
        <template v-slot:header>
            <h2>Shubrato</h2>
        </template>
        <template v-slot:main>
            <p>A Vue JS product</p>
        </template>
        <template v-slot:footer>
            <button>Buy now</button>
        </template>
    </Child1>
    <Child1>
        <template v-slot:header>
            <h2>Shubrato Kumar</h2>
        </template>
        <template v-slot:main>
            <p>A React JS product</p>
        </template>
        <template v-slot:footer>
            <button>Buy now</button>
        </template>
    </Child1>
</div>
</template>

<script>
import Child1 from "./Child1.vue"
export default {
    name: "Home",
    components:{
        Child1
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
