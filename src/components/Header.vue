<script setup>

</script>

<template>
  <div class="site-mobile-menu site-navbar-target">
    <div class="site-mobile-menu-header">
      <div class="site-mobile-menu-close">
        <span class="icofont-close js-menu-toggle"></span>
      </div>
    </div>
    <div class="site-mobile-menu-body"></div>
  </div>
  <nav class="site-nav dark js-site-navbar mb-5 site-navbar-target">
    <div class="container">
      <div class="site-navigation">
        <a href="index.html" class="logo m-0 float-left">Launch<span class="text-primary">.</span></a>
        <ul class="js-clone-nav d-none d-lg-inline-block site-menu float-left">
          <li class="active">
            <a href="#home-section" class="nav-link">Home</a>
          </li>
          <li>
            <a href="#features-section" class="nav-link">Features</a>
          </li>
          <li>
            <a href="#pricing-section" class="nav-link">Pricing</a>
          </li>
          <li>
            <a href="#about-section" class="nav-link">About</a>
          </li>
        </ul>
        <ul class="js-clone-nav d-none mt-1 d-lg-inline-block site-menu float-right">
          <li class="cta-button-outline"><a href="#">Sign in</a></li>
          <li class="cta-primary"><a href="#">Register</a></li>
        </ul>
        <a href="#" class="burger ml-auto float-right site-menu-toggle js-menu-toggle d-inline-block dark d-lg-none" data-toggle="collapse" data-target="#main-navbar">
          <span></span>
        </a>
      </div>
    </div>
  </nav>
</template>

<style scoped>

</style>