<template>
    <div class="container">
        <div class="resto">
            <div class="resto__bloc">
                <div class="resto__infos">
                    <h2>Nom resto</h2>
                    <p>tags</p>
                    <p>description Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio       nobis  magnam tenetur perferendis, enim facilis voluptates autem quae   exercitationem    voluptatum vel voluptate provident? Voluptate natus illum      nesciunt quae, aut autem?</p>
                </div>
                <div class="resto__image">
                    <img src="@/assets/img/app_store.png" alt="link_app_store">
                </div>
            </div>
            <div class="resto__menu" v-sticky="{ zIndex: 10, stickyTop: 0, disabled: false}">
                <RestoMenu/>
                <div class="basket">
                    <div class="order">Passer commande</div>
                    <div class="selection">Votre panier est vide</div>
                </div>
            </div>
            <div class="resto__list">
                <!-- DEBUT MENU ITEM -->
                <div class="menu_item">
                    <div class="menu_title">
                        <h4>Menu Item</h4>
                        <p>Item short description</p>
                    </div>
                    <div class="plat_container">
                        <!-- DEBUT LISTE PLATS -->
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <!-- FIN LISTE PLATS -->
                    </div>
                </div>
                <!-- FIN MENU ITEM -->
                <!-- MENU ITEM COPIE -->
                <div class="menu_item">
                    <div class="menu_title">
                        <h4>Menu Item</h4>
                        <p>Item short description</p>
                    </div>
                    <div class="plat_container">
                        <!-- DEBUT LISTE PLATS -->
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <div class="plat">
                                <h5>Nom plat</h5>
                                <p>description</p>
                                <p>Prix</p>
                        </div>
                        <!-- FIN LISTE PLATS -->
                    </div>
                </div>
                <!-- FIN MENU ITEM COPIE -->
            </div>
            
        </div>
    </div>
</template>

<script>
// @ is an alias to /src
import VueSticky from 'vue-sticky'
import RestoMenu from '@/components/RestoMenu.vue'

export default {
  name: 'home',
  components: {
    RestoMenu
  },
  directives: {
  'sticky': VueSticky,
}
}
</script>
<style scoped lang="scss">
.resto {
    margin: 0 auto;
    width: 1025px;
    background-color: teal;
    &__image img {
        width: 400px;
    }
    &__bloc {
        display: flex;
    }
    &__infos {
        text-align-last: left;
    }
    &__menu {
        display: flex;
        justify-content: space-between;
        border:1px solid black;
        position: relative;
    }
}
.basket {
    width: 300px;
    background-color: aquamarine;
    position: absolute;
    top: 0;
    right: 0;
}
.plat{
    display: flex;
    flex-direction: column;
    width: 340px;
    background-color: beige;
    margin-bottom: 20px;
    text-align-last: left;
    & h5, p {
        margin: 0 0 10px 0;
    }
}
.plat_container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    width: 700px;
}
.menu_title {
    text-align: left;
}
.order {
    background-color: gray;
    height: 40px;
    line-height: 40px;
}
.selection {
    height: 200px;
}
</style>
