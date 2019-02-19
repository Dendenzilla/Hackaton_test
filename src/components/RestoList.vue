<template>
  <div class="resto-pref">
    <h1>Les restaurants les mieux notés</h1>
    <div class="resto-list">
      <div class="resto">      
        <div class="img-resto healthy"></div>
        <h3>Resto title</h3>
        <p>blabla type de food</p>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'RestoList',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.resto-pref{
    background: rgb(238, 238, 238);
    padding: 70px;
}
h1{
    font-family: 'Roboto', sans-serif;
    text-align: left;
    margin-bottom: 30px;
}
</style>
