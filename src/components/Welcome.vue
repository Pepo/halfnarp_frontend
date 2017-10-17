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

 button {
     background-color: #000;
     border: none;
     color: #FFF;
     padding: 0.5rem;
     cursor: pointer;
     transition: background-color 0.5s;
     &:hover{
         transition: background-color 0.5s;
         background-color: #029319;
     }
 }
 .main__wrapper {
     max-width: 1280px;
     margin: 0 auto;
     padding: 0.5rem;
     display: flex;
     flex-wrap: wrap;
     align-items: flex-start;
     justify-content: space-between;
 }
 .main {
     margin-top: 1rem;
     padding-bottom: 3rem;
 }
</style>

<template>
  <div class="page-all-wrapper">
  	<Header></Header>
    <Navigation></Navigation>
    <main class="main">
        <div class="main__wrapper">
            <Category v-for="index in 8" :key="cat"/>
        </div>


    </main>
    <Footer />
  </div>
</template>

<script>

import Header from '../components/Header.vue'
import Navigation from '../components/Navigation.vue'
import Category from '../components/Category.vue'
import Footer from '../components/Footer.vue'

export default {
  name: 'Welcome',
  components: {
    'Header': Header,
    'Navigation': Navigation,
    'Category': Category,
    'Footer': Footer
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>
