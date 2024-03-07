<template>
<h1>Get checkbox and radio button value</h1>
<h3>Technology</h3>

<label for="java">Java</label>
<input type="checkbox" value="java" id="java" v-model="technology">

<br /><br />

<label for="php">PHP</label>
<input type="checkbox" value="php" id="php" v-model="technology">

<br /><br />

<label for="js">Javascript</label>
<input type="checkbox" value="js" id="js" v-model="technology">

<br /><br />

<h3>Who am I</h3>
<label for="student">Student</label>
<input type="radio" value="student" name="prof" id="student" v-model="who">

<label for="professional">Professional</label>
<input type="radio" value="professional" name="prof" id="professional" v-model="who">

<br /><br />

<h4>Selected technologies: {{technology}}</h4>
<br /> <br />
<h4>Profession: {{ who }}</h4>
</template>

<script>
export default {
    name: "Check Box And Radio",
    data() {
        return {
            technology: [],
            who: null
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
