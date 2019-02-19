<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <TypeFood/>
    <RestoList/>
  </div>
</template>

<script scoped>
// @ is an alias to /src
import TypeFood from '@/components/TypeFood.vue'
import RestoList from '@/components/RestoList.vue'

export default {
  name: 'home',
  components: {
    TypeFood,
    RestoList
  }
}
</script>
