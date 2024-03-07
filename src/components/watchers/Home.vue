<template>
<h1>{{ count }}</h1>
<button v-on:click="count=count+1"> + </button>
<button v-on:click="count=count-1"> - </button>
</template>

<script>
export default {

    name: "Home",
    data() {
        return {
            count: 0
        }
    },
    watch: {
        count(val) {
            if (val > 5) {
                this.count = 0;
            }

            if(val < 0){
                this.count = 0;
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
