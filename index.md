---
lang: en
permalink: /
alternate_url: /zh-hk/
---
{% assign t = site.data.i18n.en %}
<section class="hero">
	<div class="hero-badge">{{ t.home.badge }}</div>
	<h1>{{ t.home.title }}</h1>
	<p class="tagline">{{ t.home.tagline }}</p>
	<div class="download-buttons">
		<a href="#" class="badge-btn badge-apple" aria-label="{{ t.home.app_store_aria }}">
			<svg viewBox="0 0 24 24" fill="currentColor" xmlns="http://www.w3.org/2000/svg" aria-hidden="true"><path d="M18.71 19.5c-.83 1.24-1.71 2.45-3.05 2.47-1.34.03-1.77-.79-3.29-.79-1.53 0-2 .77-3.27.82-1.31.05-2.3-1.32-3.14-2.53C4.25 17 2.94 12.45 4.7 9.39c.87-1.52 2.43-2.48 4.12-2.51 1.28-.02 2.5.87 3.29.87.78 0 2.26-1.07 3.8-.91.65.03 2.47.26 3.64 1.98-.09.06-2.17 1.28-2.15 3.81.03 3.02 2.65 4.03 2.68 4.04-.03.07-.42 1.44-1.38 2.83M13 3.5c.73-.83 1.94-1.46 2.94-1.5.13 1.17-.34 2.35-1.04 3.19-.69.85-1.83 1.51-2.95 1.42-.15-1.15.41-2.35 1.05-3.11z"/></svg>
			<div class="badge-btn-inner">
				<span class="badge-btn-sub">{{ t.home.app_store_sub }}</span>
				{{ t.home.app_store_text }}
			</div>
		</a>
		<a href="#" class="badge-btn badge-google" aria-label="{{ t.home.google_play_aria }}">
			<svg viewBox="0 0 24 24" fill="currentColor" xmlns="http://www.w3.org/2000/svg" aria-hidden="true"><path d="M3.18 23.76c.37.2.8.22 1.2.06L15.55 12 11.8 8.24 3.18 23.76zM21.26 10.37l-2.7-1.54-3.37 3.17 3.37 3.17 2.72-1.55c.77-.44.77-1.81-.02-2.25zM1.64.36C1.32.67 1.13 1.15 1.13 1.79v20.42c0 .64.19 1.12.51 1.43L1.7 23.7l11.43-11.43v-.27L1.7.3 1.64.36zM15.55 12L4.38.24c-.4-.17-.83-.15-1.2.05l8.62 15.52L15.55 12z"/></svg>
			<div class="badge-btn-inner">
				<span class="badge-btn-sub">{{ t.home.google_play_sub }}</span>
				{{ t.home.google_play_text }}
			</div>
		</a>
	</div>
</section>

<section class="screenshot">
	<img src="{{ 'assets/img/mockup.png' | relative_url }}" alt="{{ t.home.screenshot_alt }}">
</section>