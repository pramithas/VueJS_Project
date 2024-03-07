<template>
<h1>{{ childUser }}</h1>
<User :getUser="getUserName" />
</template>

<script>
import User from './User.vue';

export default {
    name: "Home",
    data() {
        return {
            childUser: ""
        }
    },
    components: {
        User
    },
    methods: {
        getUserName(name) {
            this.childUser=name;
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
