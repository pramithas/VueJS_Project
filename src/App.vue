<template>
<img alt="Vue logo" src="./assets/logo.png">

<!-- <ul>
    <li v-for="user in users" :key="user.email">
        <User :data="user" :myFunc="getData" />
    </li>
</ul> -->
<!-- <User /> -->
<Home />
</template>

<script>
import Home from './components/slotswithname/Home.vue';

//import User from './components/User.vue';

export default {
    name: 'App',
    components: {
    Home
},

    data() {
        return {
            users: [{
                    name: 'Peter',
                    email: 'peter@test.com'
                },
                {
                    name: 'Sam',
                    email: 'sam@test.com'
                }, {
                    name: 'Ram',
                    email: 'ram@test.com'
                }, {
                    name: 'Rita',
                    email: 'rita@test.com'
                }
            ]
        }
    },

    methods: {
        getData(item) {
            console.warn('button clicked');
            alert("Method passed from parent for: " + item)
        }
    }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
