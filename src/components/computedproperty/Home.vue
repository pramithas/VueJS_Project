<template>
<h1>Computed Property</h1>
<!-- 1. For complex calculations, template expressions get bloated
     2. Computed properties are cached if the dependency does not change
-->
<h2>{{ (dollars*rupeeVal) - discount }}</h2>
<h2>{{ getResult }}</h2>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            dollars: 100,
            rupeeVal: 70,
            discount: 10
        }
    },

    methods: {
        getResultMethod() {
            return (this.dollars * this.rupeeVal) - this.discount;
        }
    },

    computed: {
        // This gets caches on multiple invocation.
        getResult() {
            return (this.dollars * this.rupeeVal) - this.discount;
        }
    }
}
</script>

<style>

</style>
