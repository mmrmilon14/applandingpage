<script setup>
  const HeroImage = '/images/market-launch-pana.svg';
  const AltText = 'Launch';
  const HeroTitle = 'Promote Your Products by Colorlib';
  const HeroContent = 'Another cool free html css template by <a href="#" target="_blank" class="highlight">Colorlib</a> Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast';
  const BtnFeaturesTxt = 'See Features';
  const BtnFeaturesLink = '#features-section';
  const BtnPricingTxt = 'Pricing';
  const BtnPricingLink = '#pricing-section';
</script>

<template>
  <div class="untree_co-hero" id="home-section">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12">
          <div class="dots"></div>
          <div class="row align-items-center">
            <div class="col-lg-7 ml-auto order-lg-2" data-aos="fade-right" data-aos-delay="400">
              <img :src="HeroImage" :alt="AltText" class="img-fluid">
            </div>
            <div class="col-lg-5">
              <h1 class="heading" data-aos="fade-up" data-aos-delay="0">{{ HeroTitle }}</h1>
              <div class="excerpt" data-aos="fade-up" data-aos-delay="100">
                <p v-html="HeroContent"></p>
              </div>
              <p data-aos="fade-up" data-aos-delay="200">
                <a :href="BtnFeaturesLink" class="btn btn-primary smoothscroll">{{ BtnFeaturesTxt }}</a>
                <a :href="BtnPricingLink" class="btn btn-outline-primary smoothscroll">{{ BtnPricingTxt }}</a>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>