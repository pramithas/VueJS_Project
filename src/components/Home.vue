<template>
<h1>Hey, this is the home component.</h1>

<h1>Email: {{ email }}</h1>
<h1>Phone: {{ phone }}</h1>
<h1>Name: {{ getData().email }}</h1>

<h2>Count: {{ count }}</h2>

<button v-on:click="increaseCount()">Increase Count</button>
<button v-on:dblclick="test('click me 2 button clicked twice')">Click Me 2</button>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            email: "dhakalpramithas@gmail.com",
            count: 0
        }
    },

    methods: {

        getName(name) {
            return name
        },

        increaseCount() {
            this.count++;
        },
        getData() {
            return {
                name: "Pramithas",
                email: this.email
            }
        },
        test(a) {
            alert(a);
        }

    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
