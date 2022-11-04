<template>
  <HeaderOne title="Weather App"/>
  <FooterOne author="Eric Díaz"/>
</template>

<script>
import HeaderOne from './components/HeaderOne.vue'
import FooterOne from './components/FooterOne.vue'

export default {
  name: 'App',
  components: {
    HeaderOne,
    FooterOne,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  padding: 0;
  text-decoration: none;
  box-sizing:content-box;
}
</style>
