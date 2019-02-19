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
  height: 50px;
  overflow: hidden;
  background: black;
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
