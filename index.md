---
layout: home
title: Witaj na Blisko Siebie
---

<section class="hero">
  <div class="hero-copy">
    <p class="eyebrow">W zgodzie ze Sobą</p>
    <h1>Blisko Siebie</h1>
    <p>Strona dla osób, które chcą odnaleźć wewnętrzny spokój, pewność siebie i równowagę w życiu.</p>
    <a class="button button-primary" href="/kontakt/">Umów się na konsultację</a>
  </div>
  <div class="hero-image">
    <div class="hero-shape"></div>
  </div>
</section>

<section class="section intro">
  <div class="section-grid">
    <article>
      <h2>O mnie</h2>
      <p>Jestem coachem, który wspiera Cię w podejmowaniu świadomych decyzji, osiąganiu celów i budowaniu większej pewności siebie.</p>
      <a href="/o-mnie/" class="link">Dowiedz się więcej</a>
    </article>
    <article>
      <h2>Oferta</h2>
      <p>Sesje coachingowe nastawione na zmianę, rozwój osobisty i praktyczne kroki prowadzące do lepszego życia.</p>
      <a href="/oferta/" class="link">Zobacz ofertę</a>
    </article>
    <article>
      <h2>Blog</h2>
      <p>Inspirujące artykuły o uważności, relacjach i pracy nad sobą, napisane prostym i praktycznym językiem.</p>
      <a href="/blog/" class="link">Przejdź do bloga</a>
    </article>
  </div>
</section>

<section class="section about-panel">
  <div>
    <h2>Co oferuję?</h2>
    <p>Wierzę, że każdy ma w sobie zasoby, aby żyć pełniej. Wspieram Cię w znajdowaniu swoich potrzeb, budowaniu zdrowych granic i odnajdywaniu harmonii.</p>
  </div>
</section>

<section class="section testimonials-panel">
  <div class="section-grid">
    <article class="testimonial-card">
      <p>„Czułam, że idę w złym kierunku. Dzięki coachingu poczułam większą jasność i spokój w decyzjach.”</p>
      <p class="testimonial-author">– Anna, klientka</p>
    </article>
    <article class="testimonial-card">
      <p>„Sesje pomogły mi uporządkować priorytety i rzeczywiście zacząć działać krok po kroku.”</p>
      <p class="testimonial-author">– Marta</p>
    </article>
  </div>
</section>

<section class="section featured-posts">
  <div class="section-header">
    <h2>Polecane artykuły</h2>
    <p>Praktyczne wpisy coachingowe, które warto przeczytać na start.</p>
  </div>
  <div class="posts-list">
    {% assign featured = site.posts | where: "featured", true | sort: "date" | reverse %}
    {% for post in featured limit:3 %}
    <article class="post-card">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="post-meta">{{ post.date | date: "%d %B %Y" }}</p>
      <p>{{ post.excerpt }}</p>
      <a class="link" href="{{ post.url }}">Czytaj dalej</a>
    </article>
    {% endfor %}
  </div>
</section>

<section class="section contact-panel">
  <div>
    <h2>Kontakt</h2>
    <p>Masz pytania lub chcesz zacząć pracę? Napisz do mnie, a odpowiem najszybciej jak to możliwe.</p>
    <a class="button button-secondary" href="/kontakt/">Napisz wiadomość</a>
  </div>
</section>
