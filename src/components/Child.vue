<template>
<h1>Pass data to child Component.</h1>
<h2>This is the passed name: {{ name }}</h2>
<h2>The name in object is: {{ user.name }}</h2>
<button v-on:click="getData()">Call function</button>
</template>

<script>
export default {
    name: "Child",
    props: {
        name: String,
        user: Object,
        getData:Function
    }

}
</script>

<style>
h1 {
    color: orange;
}
</style>
