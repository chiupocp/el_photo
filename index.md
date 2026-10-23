---
title: home
layout: home
type: parent
order: 1
---

<div class="section header">
	<div class="container">
		<img src="{{ "/assets/img/logo.svg" | relative_url }}">
		<h3 class="section-heading">photography</h3>
		<p class="section-description">
			Discovering the world with my vision.
		</p>
		<div id="navbar-wrapper">
			<div id="navbar">
				<img id="brand" class="hide" src="{{ "/assets/img/logo.svg" | relative_url }}">
				{% assign mypages = site.pages | where: "type", "parent" | sort: "order" %}
				{% for page in mypages %}
				<a class="button" href="{{ page.url | relative_url }}">{{ page.title }}</a>
				{% endfor %}
			</div>
		</div>
	</div>
</div>

<div class="section main">
	<div class="container">
		<div class="row" id="gallery">
  <div class="container">
    <div class="column">
      <article class="thumb">
        <img class="lazyload u-max-full-width" data-src="https://pub-725f084f4f9e40dd9cf5c2aed5a4cc84.r2.dev/5D4_0475-%E7%BC%96%E8%BE%91.jpg" alt="作品1" />
      </article>
      <article class="thumb">
        <img class="lazyload u-max-full-width" data-src="https://pub-725f084f4f9e40dd9cf5c2aed5a4cc84.r2.dev/5D4_1497-%E7%BC%96%E8%BE%91-%E7%BC%96%E8%BE%91.jpg" alt="作品2" />
      </article>
      <article class="thumb">
        <img class="lazyload u-max-full-width" data-src="https://pub-725f084f4f9e40dd9cf5c2aed5a4cc84.r2.dev/5D4_3243-%E7%BC%96%E8%BE%91-%E7%BC%96%E8%BE%91.jpg" alt="作品3" />
      </article>
    </div>
  </div>
</div>
