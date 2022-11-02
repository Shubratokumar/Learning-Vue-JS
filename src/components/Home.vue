<template>
<div>
    <h1>Get Checkbox & Radio Button Values</h1>
    <h3>Technologies</h3>
    <label for="javascript">JavaScript</label>
    <input type="checkbox" value="JavaScript" v-model="technology" id="javascript">
    <br>
    <label for="php">PHP</label>
    <input type="checkbox" value="PHP" v-model="technology" id="php">
    <br>
    <label for="swift">Swift</label>
    <input type="checkbox" value="Swift" v-model="technology" id="swift">
    <br>
    <label for="rust">Rust</label>
    <input type="checkbox" value="Rust" v-model="technology" id="rust">
    <br>
    <label for="node">Node</label>
    <input type="checkbox" value="Node" v-model="technology" id="node">
    <br>
    <br>
    <h3>Who I am </h3>
    <label for="student">Student</label>
    <input type="radio" value="Student" v-model="who" name="I" id="student">
    <br>
    <label for="developer">Frontend Developer</label>
    <input type="radio" value="Frontend Developer" v-model="who" name="I" id="developer">
    <br>
    <label for="developer1">Full Stack Developer</label>
    <input type="radio" value="Full Stack Developer" v-model="who" name="I" id="developer1">
    <br>
    <br>
    <h4>Selected Technologies: {{technology}}</h4>
    <br>
    <h4>I'm a {{who}}</h4>

</div>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            technology: [],
            who: null
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
