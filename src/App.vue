<template>
  <div>
    <Nav></Nav>
    <div id="app">
      <router-view/>
    </div>
    <Footer></Footer>
  </div>
</template>

<style lang="scss">
  @import "~bulma/sass/utilities/_all";
  @import url('https://fonts.googleapis.com/css2?family=Arimo:wght@400;700&display=swap');


  $primary: #670ddb;
  $primary-invert: findColorInvert($primary);
  $white: #FFFFFF;
  $white-invert: findColorInvert($white);

  $colors: (
          "primary": ($primary, $primary-invert),
          "white": ($white, $white-invert)
  );

  // Links
  $link: $primary;
  $link-invert: $primary-invert;
  $link-focus-border: $primary;

  $arimo: "Arimo", sans-serif;
  $family-primary: $arimo;
  $body-family: $arimo;
  h1, h2, h3, h4, h5, h6 {
    font-family: $arimo;
    font-weight: 700 !important;
  }
  $button-family: $arimo;

  $input-shadow: none;
  $input-radius: 0px;
  $button-radius: 0px;

  $sidebar-width: 50vw;

  .button {
    font-weight: 700 !important;
    margin-top: 12px;
    margin-bottom: 12px;
  }

  #app {
    max-width: 100vw;
    overflow-y: hidden;
  }

  p {
    margin-top: 12px !important;
    margin-bottom: 12px !important;
  }
  .caption {
    font-size: 16px;
    color: #888888;
  }

  .container {
    padding-left: 12px;
    padding-right: 12px;
    padding-top: 36px;
    padding-bottom: 36px;
  }

  .messageContainer {
    padding-top: 12px;
    padding-bottom: 12px;
  }

  .bbox, .bbbox {
    margin: 2.8%;
    border: solid 1px #dfdfdf;
  }

  .bbbox {
    padding: 24px;
    font-size: 18px;
  }

  .page-leave-active {
    transition: opacity 0.32s, transform 0.32s;
  }

  .page-enter-active {
    transition: opacity 0.48s, transform 0.48s;
  }

  .page-leave-to {
    opacity: 0;
  }

  .page-enter {
    opacity: 0;
    transform: translateY(-20px);
  }

  // Import Bulma and Buefy styles
  @import "~bulma";
  @import "~buefy/src/scss/buefy";
</style>

<script>
    import Nav from "./components/Nav";
    import Footer from "./components/Footer";

    export default {
        components: {Footer, Nav}
    }
</script>