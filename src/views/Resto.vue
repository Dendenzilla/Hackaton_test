<template>
<div class="fullwidth">
    <div class="container">
        <div class="resto">
            <div class="resto__bloc">
                <div class="resto__infos">
                    <h2>Pulcinella</h2>
                    <p class="tags">Cuisine italienne</p>
                    <p>Très bonnes pizzas cuites au feu de bois. Le cadre et la déco pourraient être améliorés mais ca vaut largement le déplacement ! Les pizzas sont également à emporter.</p>
                </div>
            </div>
            <div class="resto__menu" v-sticky="{ zIndex: 10, stickyTop: 0, disabled: false}">
                <RestoMenu/>
                <div class="basket">
                    <div class="order">Réserver une table</div>
                </div>
            </div>
            <div class="resto__list">
                <!-- DEBUT MENU ITEM -->
                <div class="menu_item">
                    <div class="menu_title">
                        <h4>Entrées</h4>
                        <p>Toutes nos entrées sont servies avec du pain italien bla bla bla</p>
                    </div>
                    <div class="plat_container">
                        <!-- DEBUT LISTE PLATS -->
                        <div class="plat">
                                <h5>tomates séchées</h5>
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
.fullwidth {
    width: 100vw;
    background: rgb(238, 238, 238);
}
.resto {
    margin: 0 auto;
    width: 1025px;
    &__image img {
        width: 400px;
    }
    &__bloc {
        display: flex;
    }
    &__infos {
        text-align: left;
        & h2 {
            margin-bottom: 0px;
            font-size: 30px;
        }
        & .tags {
            font-size: 12px;
            color: grey;
            font-style: italic;
        }
    }
    &__menu {
        display: flex;
        justify-content: space-between;
        position: relative;
    }
}
.basket {
    width: 300px;
    position: absolute;
    top: 0;
    right: 0;
}
.plat{
    display: flex;
    flex-direction: column;
    width: 340px;
    margin-bottom: 20px;
    text-align-last: left;
    background: white;
    padding: 5px;
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
    background: white;
    height: 40px;
    line-height: 40px;
    cursor:pointer;
}
.selection {
    height: 200px;
}
</style>
