---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---
# Example page showing switching themes

I wanted to figure out how to generate themes in Sass. Many solutions don't scale -- they don't presume you have hundreds of components written. This is a small proof-of-concept using Jekyll's Minima theme as a base. I'll make a blog post about it eventually.

## Have some example text

<h1 class="page-heading">Posts</h1>
<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="">{{ post.title | escape }}</a>
      </h2>

      {{ post.content }}
    </li>
  {% endfor %}
</ul>
