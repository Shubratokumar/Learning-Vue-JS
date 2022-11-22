<template lang="">
    <div class="cart">
        <header>
            <slot name="header"></slot>
        </header>
        <content>
            <slot name="main"></slot>
        </content>
        <footer>
            <slot name="footer"></slot>
        </footer>
    </div>
</template>

<script>
export default {
    name: "Child1"
}
</script>

<style lang="">
    .cart{
        border: 1px solid;
        width: 140px;
        text-align: center;
        padding: 20px;
    }
</style>
