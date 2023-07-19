<script setup>
  const heading = 'Pricing';
  const subHeading = 'Pricing for everyone. Choose your plan now!';
  const pricingTable = [
    {
      id: 1,
      dataDelay: 100,
      planName: 'Free',
      planPrice: 0,
      features: [
        'There live the blind texts',
        'Far far away behind the word',
        'Far from the countries Vokalia and Consonantia',
      ],
      btnLink: '#',
      btnName: 'Get Started'
    },
    {
      id: 2,
      dataDelay: 200,
      planName: 'Standard',
      planPrice: 19.99,
      features: [
        'There live the blind texts',
        'Far far away behind the word',
        'Far from the countries Vokalia and Consonantia',
      ],
      btnLink: '#',
      btnName: 'Get Started'
    },
    {
      id: 3,
      dataDelay: 300,
      planName: 'Premium',
      planPrice: 79.99,
      features: [
        'There live the blind texts',
        'Far far away behind the word',
        'Far from the countries Vokalia and Consonantia',
      ],
      btnLink: '#',
      btnName: 'Get Started'
    }
  ]
</script>

<template>
  <div class="untree_co-section bg-light" id="pricing-section">
    <div class="container">
      <div class="row pricing-title">
        <div class="col-12 text-center" data-aos="fade-up" data-aos-delay="0">
        <h2 class="heading">{{ heading }}</h2>
          <p>{{ subHeading }}</p>
        </div>
      </div>
      <div class="row justify-content-center">
        <div class="col-lg-10">
          <div class="row">

            <div v-for="(pricing, index) in pricingTable" :key="pricing.id" class="col-lg-4" data-aos="fade-up" :data-aos-delay="pricing.dataDelay">
              <div class="pricing">
                <div class="body">
                  <div class="price">
                    <span class="d-block plan">{{ pricing.planName }}</span>
                    <span class="price"><sup>$</sup><span>{{ pricing.planPrice }}</span></span>
                  </div>
                  <ul class="list-unstyled ul-check primary mb-5">
                    <li v-for="feature in pricing.features">{{ feature }}</li>
                  </ul>
                  <p class="text-center mb-0">
                    <a :href="pricing.btnLink" class="btn btn-outline-primary">{{ pricing.btnName }}</a>
                  </p>
                </div>
              </div>
            </div>

          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>