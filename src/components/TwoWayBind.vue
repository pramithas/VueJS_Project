<template>
<h1>Two way binding</h1>
<h2>{{ count }}</h2>
<input type="text" v-model="count">
</template>

<script>
export default {
    name: "Two way binding",

    data() {
        return {
            count: 0
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
