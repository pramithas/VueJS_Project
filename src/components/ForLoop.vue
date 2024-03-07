<template>
<h1>For loop in vue js</h1>

<ul>
    <li v-for="item in technologies" :key="item">
        {{ item }}
    </li>
</ul>

<br /><br />

<ul>
    <li v-for="user in users" :key="user.email">
        Name is: {{ user.name}} and email is: {{ user.email }}
    </li>
</ul>
</template>

<script>
export default {
    name: "For loop",
    data() {
        return {
            technologies: ['java', 'ruby', 'php', 'html'],
            users: [{
                name: "pramithas",
                email: "dhakalpramithas@gmail.com"
            }, {
                name: "aashma",
                email: "dahalaashma@gmail.com"
            }, {
                name: "ashmita",
                email: "dhakalashmita@gmail.com"
            }]
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
