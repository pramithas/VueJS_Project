<template>
<div class="cart">
    <header>
        <slot name="header"></slot>
    </header>
    <content>
        <slot name="main"></slot>
    </content>

    <footer>
        <slot name="footer"><button>Buy Now Default</button></slot>
    </footer>
</div>
</template>

<script>
export default {
    name: "Child"
}
</script>

<style>
.cart {
    border: 1px solid;
    width: 170px;
    text-align: center;
    padding: 20px;
}
</style>
