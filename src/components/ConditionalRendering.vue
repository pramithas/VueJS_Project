<template>
<h1 v-if="show">If else condition</h1>
<h1 v-else>Else condition</h1>
<button v-on:click="show=!show">Show</button>
</template>

<script>
export default {
    name: "If else",
    data() {
        return {
            show: false
        }
    },
    methods: {

        toggle:function(){
            this.show=!this.show
        }
    }
}
</script>

<style>

</style>
