<template>
    <div class="menu">
        <a href="#">menu item</a>
        <a href="#">menu item</a>
        <a href="#">menu item</a>
        <a href="#">menu item</a>
        <a href="#">menu item</a>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.menu {
    background-color: crimson;
    height: 40px;
    line-height: 40px;
    & a {
        text-decoration: none;
        color: black;
        margin: 0 15px 0 0;
    }
}
</style>
