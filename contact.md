---
layout: page
title: Contact Form
---

Please fill the following form with your message to contact me 

{::nomarkdown}
<form action="https://formspree.io/f/mdoyqgav" method="POST">
  <fieldset class="field">
        <input class="input" type="text" name="name" placeholder="Name" required>
        <label class="label" for="name"><span class="label-content">Your name</span></label>
    </fieldset>
    <fieldset class="field">
        <input class="input" type="email" name="_replyto" placeholder="username@domain.com" required>
        <label class="label" for="_replyto"><span class="label-content">Your email</span></label>
    </fieldset>
    <fieldset class="field">
        <textarea class="input" name="message" rows="1" placeholder="Message" required></textarea>
        <label class="label" for="message"><span class="label-content">Your message</span></label>
    </fieldset>
    <input class="hidden" type="text" name="_gotcha" style="display:none">
    <input class="hidden" type="hidden" name="_subject" value="Message via http://domain.com">
    <fieldset class="field">
        <input class="button submit" type="submit" value="Send">
    </fieldset>
</form>


{:/nomarkdown}
