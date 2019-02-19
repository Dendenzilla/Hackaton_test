<template>
    <div class="container">
        <div class="footer">
            <div class="bloc">
                <h4>Qui sommes nous</h4>
                <a href="#">Découvrir</a>
                <a href="#">L'équipe</a>
                <a href="#">Notre histoire</a>
            </div>
            <div class="bloc">
                <h4>Mentions légales</h4>
                <a href="#">Mentions légales</a>
                <a href="#">Confidentialités</a>
                <a href="#">On vend vos datas à l'Iran</a>
            </div>
            <div class="bloc">
                <h4>Télécharger</h4>
                <img src="@/assets/img/app_store.png" alt="link_app_store">
                <img src="@/assets/img/google_play.png" alt="link_google_play">
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.footer {
    background-color: rgb(37, 37, 37);
    color: white;
    display: flex;
    justify-content: space-evenly;
    margin: 0 auto;
}
.bloc {
    width: 300px;
    & a {
        text-decoration: none;
        color: white;
        display: block;
        padding: 5px 0
    }
    & img{
        width: 150px;
        display: block;
        margin: 0 auto;
    }
}
</style>
