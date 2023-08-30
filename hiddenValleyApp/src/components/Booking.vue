<!-- Component to be used in workshop page - future task -->
<template>
  <div class="booking-container">
    <div class="booking">
      <div class="booking-left">
        <div class="booking-text">Secure your spot - book now!</div>
          </div>
            <button class="button button2">Book</button>
        </div>
  </div>
</template>

<script>
  export default {
    data() {
    return {
      // You can define data properties here
    };
  },
  methods: {
    // Define methods for the booking section component
  }
  };
</script>

<style scoped>
  /* Styling for booking section */
    .booking-container {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 72px;
}

.booking {
  /* Rounded corner for booking section */
  border-radius: 8px; 
  width: 30%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #28a745;
  padding: 32px;
}

.booking-text {
  color: #F9FAF8;
  margin-left: 32px;
  font-weight: bold;
  font-size: 18px;
}

.button2 {
  margin-left: 32px;
  margin-right: 32px;
  border: 2px solid #F9FAF8;
  padding: 10px 24px;
}
</style>