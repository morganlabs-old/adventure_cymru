<script lang="ts">
  import "../styles/app.scss";
  import Navbar from "$components/layout/Navbar.svelte";
  import Footer from "$components/layout/Footer.svelte";
</script>

<div class="wrapper">
  <div class="navWrapper">
    <Navbar />
  </div>
  <div class="content">
    <slot />
  </div>
  <div class="footerWrapper">
    <Footer />
  </div>
</div>

<style lang="scss">
  .wrapper {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }

  .content {
    margin: auto;
    margin-top: 96px;
    padding-inline: 25px;
    width: 100%;
    max-width: 768px;
  }

  .footerWrapper {
    margin-top: 25px;
  }
</style>
