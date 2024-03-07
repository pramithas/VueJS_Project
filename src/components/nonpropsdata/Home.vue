<template>
<h1>Non props data</h1>
<!-- 1. No need to define type for non props data 
     2.     
-->
<User data="some data" id="user-cmp" />
</template>

<script>
import User from './User.vue';

export default {
    name: "Home",
    components: {
        User
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
