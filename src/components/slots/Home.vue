<template>
<h1>Slots in Vue js 3</h1>
<Child>
    <h1>Hey, this is Pramithas Dhakal</h1>
</Child>
<Child>
    <a href="#">Pramithas Blog Link</a>
</Child>
<!-- Default message defined in slot in Child will be displayed.-->
<Child></Child>
<Child>
    <img src="https://images.pexels.com/photos/45201/kitty-cat-kitten-pet-45201.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" /></Child>
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
