<template>
  <div id="app">
    <div class="site">
      <Header></Header>
      <Main></Main>
      <Footer></Footer>
    </div>
  </div>
</template>

<script>
    import Header from './components/Header'
    import Main from './components/Main'
    import Footer from './components/Footer'

    export default {
        name: 'app',
        components: {
            'Header': Header,
            'Main': Main,
            'Footer': Footer
        }
    }
</script>

<style src="./styles.scss" lang="scss"></style>
