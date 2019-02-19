<template>
  <div class="header">
    <nav class="container">
      <a class="logo">
        <i class="fas fa-hamburger"></i> Eat.brussels
      </a>
      <ul>
        <li>
          <a href="#" class="link-menu">Se connecter</a>
        </li>
        <li>
          <a href="#" class="link-menu">S'inscrire</a>
        </li>
      </ul>
    </nav>
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
export default {};
</script>

<style>
/* nav */
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
}
.logo {
  font-family: "Roboto", sans-serif;
  font-weight: bold;
  font-size: 17px;
}
ul {
  display: flex;
}
li {
  list-style: none;
}
.link-menu {
  color: white;
  text-decoration: none;
  margin-left: 25px;
}
/* head */
.header {
  margin: 0;
  position: relative;
  max-width: 100vw;
  height: 500px;
  overflow: hidden;
  background: url("~@/assets/img/head-img.jpg") center/cover;
}
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
  width: 450px;
  margin-top: 150px;
}

@media screen and (max-width: 1150px) {
  .head-intro {
    margin-top: 0;
  }
}
@media screen and (max-width: 770px) {
  .header {
    height: 450px;
  }
  .title {
    font-size: 1.6em;
  }
  .search-bar {
    width: 85%;
  }
  .head-intro {
    width: 90%;
    margin-top: 150px;
  }
}
</style>
