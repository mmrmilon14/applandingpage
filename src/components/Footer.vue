<script setup>
  const overview = 'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.';
  const navigations = [
    {
      id: 1,
      menuTitle: 'Projects',
      menus: [
        'La Lega Stadium',
        'France Building',
        '22 New Homes',
        'Manage Center',
        'Sports Hall',
      ]
    },
    {
      id: 2,
      menuTitle: 'Services',
      menus: [
        'Architect',
        'Interior Design',
        'Landscape Design',
        'Consultancy'
      ]
    },
    {
      id: 3,
      menuTitle: 'Contact',
      address: '43 Raymouth Rd. Baltemoer, London 3910',
      menus: [
        '+1(123)-456-7890',
        '+1(123)-456-7890',
        'info@mydomain.com'
      ]
    }
  ]

</script>

<template>
  <div class="site-footer">
    <div class="footer-dots"></div>
    <div class="container">
      <div class="row">
        <div class="col-lg-4">
          <div class="widget">
            <h3>About Launch<span class="text-primary">.</span> </h3>
            <p>{{ overview }}</p>
          </div>
        </div>
        <div v-for="(navigation, index) in navigations" :key="navigation.id" class="col-lg-2" :class="1==navigation.id?'ml-auto':''">
          <div class="widget">
            <h3>{{ navigation.menuTitle }}</h3>
            <address v-if="3==navigation.id">{{ navigation.address }}</address>
            <ul class="list-unstyled float-left links">
              <li v-for="menu in navigation.menus"><a href="#">{{ menu }}</a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="row mt-5">
        <div class="col-12 text-center">
          <p>Copyright &copy; 2023 All rights reserved
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>