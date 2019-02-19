<template>
    <div class="menu">
        <a href="#">Entrées</a>
        <a href="#">Plats</a>
        <a href="#">Spécialités</a>
        <a href="#">Desserts</a>
        <a href="#">Vins</a>
        <a href="#">Boissons</a>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.menu {
    height: 40px;
    background-color:rgb(238, 238, 238);
    width: 100%;
    display: flex;
    align-items: baseline;
    & a {
        text-decoration: none;
        color: black;
        margin: 0 15px 0 0;
        color: coral;
        border-bottom: 2px dotted coral;
        font: 20px bold;
    }
}
</style>
