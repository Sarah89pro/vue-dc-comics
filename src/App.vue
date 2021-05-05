<template>
<div id="app">
  <!--HEADER-->
  <Header/>
  <!--MAIN CONTENT-->

  <!--FOOTER-->

</div>
</template>

<script>
import Header from '../src/components/Header'

export default {
  name: 'App',
  components: {
    Header,

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


.container {
  max-width: 1200px;
  margin: 0 auto;
}
</style>
