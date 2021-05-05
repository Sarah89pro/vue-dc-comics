<template>
<div id="app">
  <!--HEADER-->
  <Header/>
  <!--MAIN CONTENT-->
  <Hero/>
  <Main/>
  <!--FOOTER-->
  <Links/>
  <Footer/>


</div>
</template>

<script>
import Header from '../src/components/Header'
import Hero from '../src/components/Hero'
import Main from '../src/components/Main'
import Links from '../src/components/Links'
import Footer from '../src/components/Footer'



export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Main,
    Links,
    Footer
  }
}
</script>

<style lang="scss">

/*GENERAL*/ 
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


body {
  font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}


a {
  text-decoration: none;
}


ul {
  list-style: none;
}

img {
  max-width: 100%;
}

.container {
  display: flex;
  max-width: 1200px;
  margin: 0 auto;
}
</style>
