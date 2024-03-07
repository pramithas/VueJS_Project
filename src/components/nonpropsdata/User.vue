<template>
<!-- 1. If this div was not there, the id would not be added to any h3 tag 
     2. To bind the attribute with particular tag, we should use v-bind attr-->
<div>
    <h3 v-bind="$attrs">Peter</h3>
    <h3 v-bind="$attrs">Bruce</h3>
    <h3>Anil</h3>
    <h3>{{ data }}</h3>
</div>
</template>

<script>
export default {
    name: "User",
    // Do not inherit in div by default
    inheritAttrs: false,
    props: {
        data: String,
        // Nothing will be bind because we have defined it as a prop.
        id: String
    }
}
</script>

<style>

</style>
