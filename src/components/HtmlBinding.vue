<template>
<div v-html="tag"></div>
<div v-html="tag2"></div>
</template>

<script>
export default {

    data() {
        return {
            tag: "<h1>Hello World</h1>",
            tag2:"<h1>dhakalpramithas@gmail.com</h1>"
        }
    }

}
</script>

<style>

</style>
