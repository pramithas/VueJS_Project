<template>
<Child>
    <template v-slot:header>
        <h1>Pramithas</h1>
    </template>

    <template v-slot:main>
        <p>A Vue JS Project</p>
    </template>

    <template v-slot:footer><button>Buy Now</button></template>
</Child>

<Child>
    <template v-slot:header>
        <h1>Aashma</h1>
    </template>

    <template v-slot:main>
        <p>A React JS Project</p>
    </template>

    <template v-slot:footer></template>
</Child>
</template>

<script>
import Child from "./Child.vue";

export default {
    name: "Home",
    components: {
        Child
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
