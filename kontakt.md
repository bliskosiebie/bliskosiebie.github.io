---
layout: default
title: Kontakt
permalink: /kontakt/
---

<section class="page-header">
  <h1>Kontakt</h1>
  <p>Napisz wiadomość, by umówić się na konsultację lub dowiedzieć się więcej o ofercie.</p>
</section>

<section class="section contact-form-section">
  <form action="https://formspree.io/f/your-form-id" method="POST">
    <label for="name">Imię</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email</label>
    <input type="email" id="email" name="email" required>

    <label for="message">Wiadomość</label>
    <textarea id="message" name="message" rows="6" required></textarea>

    <button type="submit" class="button button-primary">Wyślij wiadomość</button>

  </form>
  <div class="contact-details">
    <h2>Masz pytanie?</h2>
    <p>kontakt@bliskosiebie.pl</p>
    <p>Spotkania online</p>
  </div>
</section>

<p class="note">Uwaga: aby formularz działał, zastąp <code>your-form-id</code> swoim identyfikatorem Formspree lub skonfiguruj inny serwer pocztowy.</p>
