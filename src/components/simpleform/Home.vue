<template>
<h1>Simple Form</h1>

<ul>
    <li v-for="item in error" :key="item">
        {{ item }} not valid.
    </li>
</ul>

<form>
    <label>Email : </label>
    <input type="text" placeholder="Enter Email" v-model="form.email">
    <br /> <br />

    <label>Password : </label>
    <input type="password" placeholder="Enter a password" v-model="form.password" />
    <br /> <br />

    <label>Country : </label>
    <select v-model="form.country">
        <option>India</option>
        <option>China</option>
        <option>USA</option>
    </select>

    <h2>Technologies : </h2>
    <label>Java</label>
    <input type="checkbox" value="java" v-model="form.technologies" />
    <br /> <br />

    <label>Python</label>
    <input type="checkbox" value="PYTHON" v-model="form.technologies" />
    <br /> <br />

    <label>PHP</label>
    <input type="checkbox" value="PHP" v-model="form.technologies" />
    <br /> <br />

    <h2>Gender</h2>

    <label>Male</label>
    <input type="radio" value="Male" name="gender" v-model="form.gender" />
    <br /> <br />

    <label>Female</label>
    <input type="radio" value="Female" name="gender" v-model="form.gender" />
    <br /> <br />

    <button type="button" v-on:click="login()">Login</button>

</form>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            form: {
                email: 'rita@gmail.com',
                password: '',
                country: '',
                technologies: [],
                gender: ''
            },
            error: []
        }
    },

    methods: {
        login() {
            this.error = [];

            for (const item in this.form) {
                if (this.form[item] === "" || this.form[item].length === 0) {
                    this.error.push(item);
                }
            }

            console.warn(this.error);

            if (this.error.length === 0) {
                alert("The form has been successfully submitted.")
            }
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
