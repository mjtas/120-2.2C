<template>
  <div class="header">
    <div class="header-text">
      <button class="header-link-toggle" @click="toggleHeader"><img src="../assets/header_toggle.png"></button>
      <!-- Left side links -->
      <ul class="header-ul header-ul-left" :class="{ displayHeaderLinks: displayHeaderLinks }">
        <li class="header-li"><a class="header-a" href="#">Home</a></li>
        <li class="header-li"><a class="header-a" href="#">About Us</a></li>
        <li class="header-li"><a class="header-a" href="#">Workshops</a></li>
        <li class="header-li"><a class="header-a" href="#">Gift Vouchers</a></li>
      </ul>
      <!-- Right side links -->
      <ul class="header-ul header-ul-right" :class="{ displayHeaderLinks: displayHeaderLinks }">
        <li class="header-li"><a class="header-a" href="#">Picnic Hampers</a></li>
        <li class="header-li"><a class="header-a" href="#">Blog</a></li>
        <li class="header-li"><a class="header-a" href="#">Contact Us</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      displayHeaderLinks: false, // Flag to control the display of header links
    };
  },
  methods: {
    toggleHeader() {
      this.displayHeaderLinks = !this.displayHeaderLinks; // Toggle the value of 'displayHeaderLinks' property
    }
  }
}
</script>