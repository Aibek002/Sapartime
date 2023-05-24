<template>
  <div id="body">
    <HeaderComp />
    <ContentsComp />
  </div>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue"
import ContentsComp from "./components/ContentComp.vue"

export default {
  components: {
    HeaderComp, ContentsComp
  }
}
</script>

<style></style>
