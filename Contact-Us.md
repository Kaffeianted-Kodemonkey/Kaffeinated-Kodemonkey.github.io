---
layout: template
meta-title: Contact Us
title: Contact Us
subtitle: Questions & Comments
category: Frequently Asked Questions
mine-image: contact-us.png
img-size: 100
description: Website contact form
permalink: Contact-Us
---

<div class="row">
  <div class="col-6">
    <form accept-charset="UTF-8" action="https://formspree.io/admin@kaffeinatedkodemonkey.com" method="POST">
      <div class="form-group">
        <input type="text" class="form-control" aria-label="Name" name="name" placeholder="first name" required>
      </div>

      <div class="form-group">
          <input type="email" class="form-control" aria-label="Email" name="email" placeholder="Email" required>
      </div>


      <div class="form-group">
          <textarea class="form-control" aria-label="Message" name="message" rows="8" placeholder="Message"></textarea>
      </div>

      <div class="center-content">
          <input type="submit" value="Submit" class="btn btn-md btn-info">
      </div>
    </form>
  </div>
  <div class="col-5">
    <p>We have developers and marketers standing by to help you with your next project.</p>
    <p>If you have a question about one of our packages please don't hesitate to ask.</p>

    <div class="contact_address margin-top-40">
        <p><abbr title="Location" class="initialism">Loc: Rangely, Colorado</abbr></p>
        <p><abbr title="Phone" class="initialism">P: (720) 608-1444</abbr></p>>
    </div>

    <div class="social-icon">
      <a class="nav-link" href="https://facebook.com/{{site.facebook_username}}" target="_blank" title="Facebook" aria-label="facebook"><i class="fab fa-facebook-f"></i></a>
      <a class="nav-link" href="https://twitter.com/{{site.twitter_username}}" target="_blank" title="Twitter" aria-label="twitter"><i class="fab fa-twitter"></i></a>
      <a class="nav-link" href="https://www.linkedin.com/in/{{site.linkedIn_username}}" target="_blank" title="LinkedIn" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
    </div>
  </div>
</div>
