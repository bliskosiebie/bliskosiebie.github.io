---
layout: default
title: Kontakt
permalink: /kontakt/
---

<section class="page-header">
  <h1>Kontakt</h1>
  <p>Podaj tylko imię i email, a skontaktuję się z Tobą w sprawie coachingu.</p>
</section>

<section class="section contact-form-section">
  <form action="https://formspree.io/f/your-form-id" method="POST">
    <label for="name">Imię</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email</label>
    <input type="email" id="email" name="email" required>

    <input type="hidden" name="_subject" value="Prośba o kontakt coachingowy">
    <input type="hidden" name="message" value="Osoba prosi o kontakt w sprawie coachingu.">

    <button type="submit" class="button button-primary">Poproś o kontakt coachingowy</button>
  </form>

  <div class="contact-details">
    <h2>Chcesz szybszy kontakt?</h2>
    <p>Wyślij wiadomość bezpośrednio na Messenger:</p>
    <a class="button button-secondary" href="https://m.me/TwojaNazwa" target="_blank" rel="noopener">Napisz na Messengerze</a>
    <p class="small-note">Zastąp <code>https://m.me/TwojaNazwa</code> linkiem do swojej strony na Messengerze.</p>
  </div>
</section>

<p class="note">Uwaga: aby formularz działał, zastąp <code>your-form-id</code> swoim identyfikatorem Formspree lub skonfiguruj inny serwer pocztowy.</p>
