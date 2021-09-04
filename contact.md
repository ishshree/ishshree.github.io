---
layout: content
---

<div class="form-box">
  <div class="contact-head">
    {% if site.data.settings.contact.description %}
      <p class="page-description">{{site.data.settings.contact.description}}</p>
    {% endif %}
  </div>
  <form class="form" action="https://formspree.io/f/{{site.mail}}" method="POST">
    <div class="form__group">
      <label class="form__label screen-reader-text" for="form-name">Your Name/आपका नाम</label>
      <input class="form__input" id="form-name" type="text" name="name" placeholder="Your Name/आपका नाम" required>
    </div>
    <div class="form__group">
      <label class="form__label screen-reader-text" for="form-email">Your Email/आपका ईमेल</label>
      <input class="form__input" id="form-email" type="email" name="_replyto" placeholder="Your Email/आपका ईमेल" required>
    </div>
    <div class="form__group">
      <label class="form__label screen-reader-text" for="form-text">Your Message/आपका संदेश</label>
      <textarea class="form__input" id="form-text" name="text" rows="10" placeholder="Message/संदेश" required></textarea>
    </div>
    <div class="form__group">
      <button class="button" type="submit">Send Message/संदेश भेजें</button>
    </div>
  </form>
</div>