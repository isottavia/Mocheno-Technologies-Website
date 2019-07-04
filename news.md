---
layout: page
title: News
permalink: /news/
---

<br>
<div class="album py-5 bg-light">
    <div>
        {% for post in site.posts %}
        <div class="row">
	        <div class="col-md-9">
	        	<div class="card text-white bg-dark mb-3">
						<div class="card-header"><small class="text-muted">{{ post.date | date: "%b %-d, %Y" }}</small></div>
						<div class="card-body">
						<h5 class="card-title"><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h5>
							<p class="card-text">{{ post.tagline }}</p>
						</div>
				</div>
			</div>
			<div class="col-md-3">
	        	<img src="{{ site.baseurl }}/{{ post.imgThumbnail }}" alt="Smiley face" class="rounded-circle">
			</div>
		</div>
		<br>
		{% endfor %}
    </div>
</div>   

<br>