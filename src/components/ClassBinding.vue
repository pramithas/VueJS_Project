<template>
<h1>CSS binding</h1>
<h2 :class="applyStyle">Home Component</h2>
<button v-on:click="colorful=!colorful">Click to toggle color</button>
</template>

<script>
export default {

    name: "Home",

    data() {
        return {
            colorful: false
        }
    },
    computed: {
        applyStyle() {
            return {
                green: this.colorful,
                err: true
            }
        }
    }

}
</script>

<style scoped>
h1 {
    color: orange;
}

.green {
    background-color: green;
    width: 200px;
    padding: 10px;
}

.err {
    color: red;
}
</style>
