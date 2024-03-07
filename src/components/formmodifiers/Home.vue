<template>
<h1>Form Modifiers</h1>
<!-- v-model.lazy, v-model.trim, v-model-number //set the type explicitely.
    Can use more than one modifier together such as: v-model.number.lazy="data"
-->
<input type="number" v-model.lazy="data" />
<h2>Data is: {{ typeof data }}</h2>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            data: ''
        }
    }
}
</script>

<style>

</style>
