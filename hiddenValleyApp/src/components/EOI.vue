<!-- Component to be used in workshop page - future task -->
<template>
    <div class="EOI">
      <!--Example form-->
      <form class="interest-form">
      <h3>Subscribe to keep up to date</h3>
        <label for="name">Name:</label><br>
        <input type="text" id="name" name="name"><br>
        <label for="user_email">Email Address:</label><br>
        <input type="email" id="user_email" name="email" placeholder="you@example.com"><br>
        <fieldset>
	        <legend>I would like to learn more about:</legend>
          <input type="checkbox" id="no_dig" name="interest_area" value="no_dig" checked>
          <label for="no_dig">No dig gardening</label>
          <input type="checkbox" id="bread" name="interest_area" value="bread" checked>
          <label for="bread">Bread making</label>
          <input type="checkbox" id="building" name="interest_area" value="building" checked>
          <label for="building">Building</label>
        </fieldset>
        <button type="submit" class = "button button1">Subscribe</button>
      </form>
	  </div>                  
  </template>
  
  <script>
  export default {
    // Component logic here
  };
  </script>
  