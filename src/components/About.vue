<script setup>
  const aboutImage = '/images/about.svg';
  const AltText = 'Launch';
  const heading = 'About';
  const subHeading = 'About Us';
  const content = 'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast';
  const contentHtml = 'Separated they <span class="highlight">live in Bookmarksgrove right at the coast of the Semantics</span>, a large language ocean. A small river named Duden flows by their place and supplies it with the necessary regelialia.';
  const lists = [
    'There live the blind texts',
    'Far far away behind the word',
    'Their place and supplies'
  ];
  const aboutInfos = [
    {
      id: 1,
      dataDelay: 0,
      dataNumber: 59,
      dataText: 'M',
      dataName: 'Members'
    },
    {
      id: 2,
      dataDelay: 100,
      dataNumber: 14,
      dataText: '',
      dataName: 'Team'
    }
  ]
</script>

<template>
  <section class="untree_co-section" ref="about-section" id="about-section">
    <div class="container">
      <div class="row justify-content-between">
        <div class="col-lg-8" data-aos="fade-up" data-aos-delay="100">
          <img :src="aboutImage" :alt="AltText" class="img-fluid">
        </div>
        <div class="col-lg-4">
          <div class="mb-4" data-aos="fade-up" data-aos-delay="0">
            <span class="caption">{{ heading }}</span>
            <h2 class="heading">{{ subHeading }}</h2>
          </div>
          <div class="mb-4" data-aos="fade-up" data-aos-delay="100">
            <p>{{ content }}</p>
            <p v-html="contentHtml"></p>
          </div>
          <ul class="list-unstyled ul-check primary mb-4" data-aos="fade-up" data-aos-delay="200">
            <li v-for="(list, index) in lists" :key="index">{{ list }}</li>
          </ul>
          <div class="row count-numbers">
            <div v-for="(aboutInfo, index) in aboutInfos" :key="aboutInfo.id" class="col-lg-6" data-aos="fade-up" :data-aos-delay="aboutInfo.dataDelay">
              <span class="counter d-block"><span :data-number="aboutInfo.dataNumber">{{ aboutInfo.dataNumber }}</span><span>{{ aboutInfo.dataText }}</span></span>
              <span class="caption-2">{{ aboutInfo.dataName }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
</style>