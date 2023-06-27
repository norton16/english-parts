<template>
  <HeaderBar />
  <SearchBar />
  <HeroSection />
  <SelectMake />
  <SelectCategory />
  <FooterBar />
</template>

<script>
import HeaderBar from './components/HeaderBar.vue'
import SearchBar from './components/SearchBar.vue'
import HeroSection from './components/HeroSection.vue'
import SelectMake from './components/SelectMake.vue'
import SelectCategory from './components/SelectCategory.vue'
import FooterBar from './components/FooterBar.vue'

export default {
  name: 'App',
  components: {
    HeaderBar,
    SearchBar,
    HeroSection,
    SelectMake,
    SelectCategory,
    FooterBar
  }
}
</script>

<style lang="less">
#app {
  font-family: verdana, sans-serif;
  margin: auto;
  overflow-x: hidden;
}
body {
  margin: 8px 0px;
}
</style>
