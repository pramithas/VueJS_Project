<template>
<div class="udata">
    <h2>{{ data.name }}</h2>
    <h2>{{ data.email }}</h2>
    <button v-on:click="myFunc(data.name)">Alert Name</button>
</div>
</template>

<script>
export default {

    props: {
        data: Object,
        myFunc: Function
    }

}
</script>

<style>
.udata {
    background-color: skyblue;
    padding: 10px;
    border-bottom: 1px solid;
    margin-bottom: 20px;
}
</style>
