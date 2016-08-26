---
layout: splash
permalink: /
header:
  overlay_color: "#5e616c"
  overlay_image: mm-home-page-feature.jpg
  cta_label: "<i class='fa fa-book'></i> Read the principals"
  cta_url: "/principals/"
  caption:
excerpt: 'A flexible two-column Jekyll theme. Perfect for personal sites, blogs, and portfolios hosted on GitHub or your own server.<br /> <small><a href="https://github.com/mmistakes/minimal-mistakes/releases/tag/3.4.4">Latest release v3.4.4</a></small><br /><br /> {::nomarkdown}<iframe style="display: inline-block;" src="https://ghbtns.com/github-btn.html?user=mmistakes&repo=minimal-mistakes&type=star&count=true&size=large" frameborder="0" scrolling="0" width="160px" height="30px"></iframe> <iframe style="display: inline-block;" src="https://ghbtns.com/github-btn.html?user=mmistakes&repo=minimal-mistakes&type=fork&count=true&size=large" frameborder="0" scrolling="0" width="158px" height="30px"></iframe>{:/nomarkdown}'
feature_row:
  - image_path: mm-customizable-feature.png
    alt: "customizable"
    title: "Code Tutorial"
    excerpt: "Everything from the menus, sidebars, comments, and more can be configured or set with YAML Front Matter."
    url: "/code-tutorial/"
    btn_label: "Learn More"
  - image_path: mm-responsive-feature.png
    alt: "fully responsive"
    title: "Other tutorial"
    excerpt: "Built on HTML5 + CSS3. All layouts are fully responsive with helpers to augment your content."
    url: "/other-tutorial/"
    btn_label: "Learn More"
  - image_path: mm-free-feature.png
    alt: "100% free"
    title: "Third Tutorial"
    excerpt: "Free to use however you want under the MIT License. Clone it, fork it, customize it, whatever!"
    url: "/third-tutorial/"
    btn_label: "Learn More"
github:
  - excerpt: '{::nomarkdown}<iframe style="display: inline-block;" src="https://ghbtns.com/github-btn.html?user=mmistakes&repo=minimal-mistakes&type=star&count=true&size=large" frameborder="0" scrolling="0" width="160px" height="30px"></iframe> <iframe style="display: inline-block;" src="https://ghbtns.com/github-btn.html?user=mmistakes&repo=minimal-mistakes&type=fork&count=true&size=large" frameborder="0" scrolling="0" width="158px" height="30px"></iframe>{:/nomarkdown}'
intro:
  - excerpt: 'Get notified when I add new stuff &nbsp; [<i class="fa fa-twitter"></i> @mmistakes](https://twitter.com/mmistakes){: .btn .btn--twitter}'
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

<h1>The Principals</h1>
{% for collection in site.collections %}

  {% for post in collection.docs %}
    {% if collection.label == "principals" %}
      {% include archive-single.html %}
    {% endif %}
  {% endfor %}
{% endfor %}
