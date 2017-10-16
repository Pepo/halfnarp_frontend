<style lang="scss">
 body, html, * {
    margin: 0;
    padding: 0;
    font-family: sans-serif;
    box-sizing: border-box;
 }
 body {
     font-size: 20px;
     line-height: 1.3;
 }
 .page-wrapper {
     max-width: 1280px;
     margin: 0 auto;
     padding: 0.5rem;
 }
 .main {
     margin-top: 1rem;
 }
 .category {
     max-width: 33%;
 }
</style>

<template>
  <div class="page-all-wrapper">
  	<Header></Header>
    <Navigation></Navigation>
    <main class="main">
        <div class="page-wrapper">
            <Category />
        </div>
    </main>
  </div>
</template>

<script>

import Header from '../components/Header.vue'
import Navigation from '../components/Navigation.vue'
import Category from '../components/Category.vue'

export default {
  name: 'Welcome',
  components: {
    'Header': Header,
    'Navigation': Navigation,
    'Category': Category
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>
