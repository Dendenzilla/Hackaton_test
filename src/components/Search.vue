<template>
    <div class="fullwidth">
    <div class="container">
      <div class="head-intro">
        <h1 class="title">Les meilleurs restaurants près de chez vous.</h1>
        <div class="search">
          <input type="text" name="adress" id class="search-bar" placeholder="Votre adresse">
          <div class="loupe-bg">
            <i class="fas fa-search"></i>
          </div>
        </div>
      </div>
    </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.title {
    font-family: "Roboto", sans-serif;
    color: white;
    text-align: left;
}
.img-head {
    z-index: -2;
}
.search {
    display: flex;
    align-items: center;
}
.search-bar {
    background: white;
    padding: 15px;
    border: none;
    height: 40px;
    width: 440px;
    margin: 0;
    left: 0;
}
.loupe-bg {
    cursor: pointer;
    background: crimson;
    height: 40px;
    width: 45px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.fa-search {
    color: white;
}
.head-intro {
    height: 450px;
    width: 100vw;
}
.fullwidth {
    width: 100vw;
    background: url("~@/assets/img/head-img.jpg") center/cover;
}
</style>
