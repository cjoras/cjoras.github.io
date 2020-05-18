---
#Front Matter

title: Christer Jorås - Hjem
layout: default
---
<section id="welcome-section">
    <h1>Hei! Jeg er <em>Christer Jorås</em>!</h1>
    <p>Jeg utvikler nettsider, og i tillegg er jeg en <span class='random-text'></span></p>
    <p>Ta en titt på de siste prosjektene mine nedenfor</p>
    <a href='#projects'><div id='icon-downarrow-main'></div></a>
  </section>
  <section id="projects">
    {% for post in site.posts %}
    <div class='project-tile'>
      <img class='thumbnail' src='{{ post.thumbnail }}'>
      <a href="{{ post.url }}">
        <div class='text-container'>
          <h2 class='project-title'>{{ post.title }}</h2>
          <p class='project-description'>{{ post.excerpt }}</p>
        </div>
      </a>
    </div>
    {% endfor %}
  </section>