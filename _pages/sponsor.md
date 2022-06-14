---
layout: page
title: Sponsor
permalink: /sponsor
comments: false
---


<script type="text/javascript">var submitted=false;</script>
<script type="text/javascript">
//$('#gform').on('submit', function(e) {
//  $('#gform *').fadeOut(2000);
//  $('#gform').prepend("Thank you for your sponsorship! If you haven't already, please send your donation of any amount to my Dads <a href='https://paypal.me/andyboot' target='_blank'>PayPal (click here)</a>.");
//  });
  
  
window.addEventListener("load", function() {
  const form = document.getElementById('gform');
  form.addEventListener("submit", function(e) {
    e.preventDefault();
    const data = new FormData(form);
    const action = e.target.action;
    fetch(action, {
      method: 'POST',
      body: data,
    })
    .then(() => {
      $('#gform *').fadeOut(2000);
      $('#gform').prepend("Thank you for your sponsorship! If you haven't already, please send your donation of any amount to my Dads <a href='https://paypal.me/andyboot' target='_blank'>PayPal (click here)</a>.");
    })
  });
});  
</script>

<form name="gform" id="gform" method="POST" action="https://script.google.com/macros/s/AKfycbwRFvtpfJc9xs0G_KP-BELHVkP2FLvde_BM42k7f-w2ORsUZGuaNjSuQ7aoGSHqwBpkzA/exec">
  <div class="container">
    <div class="row">
      <div class="col-sm">
        <div class="form-group">
          <label for="FirstName">First Name</label>
          <input type="text" class="form-control form-control-lg" id="FirstName" name="FirstName" placeholder="Enter first name" required>
          <small id="emailHelp" class="form-text text-muted">This will be what is shown in the gallery.</small>
        </div>
      </div>
      <div class="col-sm">
        <div class="form-group">
          <label for="LastName">Last Name</label>
          <input type="text" class="form-control form-control-lg" id="LastName" name="LastName" placeholder="Enter last name" required>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-sm">
        <div class="form-group">
          <label for="EmailAddress">Email address</label>
          <input type="email" class="form-control form-control-lg" id="EmailAddress" name="EmailAddress" aria-describedby="emailHelp" placeholder="Enter email" required>
          <small id="emailHelp" class="form-text text-muted">I'll never share your email with anyone else.</small>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-sm">
        <div class="form-group">
          <label for="Address">Address</label>
          <input type="text" class="form-control form-control-lg" id="Address" name="Address" aria-describedby="emailHelp" placeholder="Enter postal address">
          <small id="emailHelp" class="form-text text-muted">For GiftAid. Leave blank to opt out.</small>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-sm">
        <div class="form-group">
          <label for="PictureRequest">Your picture request</label>
          <input type="text" class="form-control form-control-lg" id="PictureRequest" name="PictureRequest" placeholder="Please provide full description">
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-sm">
        <button type="submit" class="btn btn-primary btn-lg">Submit</button>
      </div>
    </div>
  </div>  
</form>
<iframe name="hidden_iframe" id="hidden_iframe" style="display:none;" onload="if(submitted) {}"></iframe>

