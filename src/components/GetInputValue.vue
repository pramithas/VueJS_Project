<template>
<h1>Get Input field value</h1>
<input type="text" placeholder="Enter email" v-model="email">
<br /><br />
<input type="text" placeholder="Enter password" v-model="password">
<br /><br />
<button v-on:click="getData()" type="button">Get Values</button>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            email: null,
            password: null
        }
    },
    methods: {

        getData() {
            console.warn("The values are:", this.email, this.password);
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
